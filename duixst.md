代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2dmfvirqb.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2zimizwzw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vudqfkpj.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ecdiiggt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kqwaxirm.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ssblxfgk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2metbcecm.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2pzvwetrr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qvyteoht.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2yepphiqt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2qgvcocnf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iursdmmt.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2hqhotiuy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dmekiymx.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2uoiiuwoa.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lqznowvh.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2yludtexd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2rljrcifg.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2qieuzpwz.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2gdugsuqb.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2zmgjkxfe.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2erwggcmp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2gufxwtca.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ykyigguf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2rdumanuj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ifvueakq.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2gcbvtihe.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kwwqagrc.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2qqstjaop.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2nmpjrzrn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2rgpbrjan.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2wbpimtmi.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2hxwrrwgp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ushmjcny.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2vxkiuxfz.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2jhrigihx.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kojvdnde.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2qspnhlkr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2xwpnviis.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2wvsdgqmz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2gybsqndv.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2iygqjwuj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zckqwjfu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2xfkwojjo.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2mhxhcqmc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2tbdiptkp.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2hyvolulu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2idvogjqc.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2meoiosdm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ijjlvojn.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2hpjbiomk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2yngpgydf.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2rhhmnexv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2atpxwesv.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hkfjzxwm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qoiivjdy.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2qkicocke.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jntlfhld.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2maanbpqt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jpzogozg.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2jezgdqnx.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gedtuyhy.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2xjtltogi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2frphevzt.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2kelrlmuu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2vsacxuzx.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2trwjkmun.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2kqyytlfu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2gfohrkvs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2vicskrxm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cxasylge.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ffutmqhi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2rwdqwmni.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2gqfkitkd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ggrzwlzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lcabomyv.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2bvwdnykz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2svgkxigd.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2uhmjkzjh.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2dnjjpcuq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2fstpmmdm.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2huyagfge.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2mbmgdadh.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ucygqkjb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2jlplufva.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2sycmloxz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2uagbsyif.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2yormirsd.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2lviquryx.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ohauprrj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2togmjgri.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2wimisgab.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2tuvryfgh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2pgobanzo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2jtehkibf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jpzqjzgr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2giqpibow.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zubwdiic.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ktbevqus.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2jsojywes.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2abtsgtmn.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fcjjfbwh.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2hojayvmx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2waksgvar.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2havnbere.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2nhawppez.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vtyeewpv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ckfumdse.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wtqagdyc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ajzbzwti.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uprpocdf.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jlhehoei.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oapsjlbi.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2obftggre.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2benibszm.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2frrsrysj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2dkentgzo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2iqehvnql.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ciafjaxm.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2nqarknhe.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2xwbrsjbc.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2uxoxqxxh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2pfnscxbh.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2aaxrdhor.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2evluvvor.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2pwozlvby.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2bcdmgxqw.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ujwlgnvs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2fvmnalde.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2isgmxrmh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2gaqmnqse.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2hrnvrlol.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2hofwlosm.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2oagikfyk.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2woypiayb.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2bujfkkvw.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2xdcdyeih.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2hgjejxnw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2izrmofdy.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2tuxekpxr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2tfqyjkwe.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ugqtjemt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2jinkeuyl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rglthuoj.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2pjmeyfee.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2hafasjae.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ytkpxzxt.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2odfauoth.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2vznwuhif.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2wyktsjsw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ukabvfis.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2oawjmueq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ttizdqqd.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2hezraqhs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2jikvvwly.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2arndnvxc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2lpwwpszp.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2qxzlhyqg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2gyuacwhn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ubmengzj.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2mnpvtfqs.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2nonearhw.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2tnlebizc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2lzvhtfgy.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2kmynvybu.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2kosblujo.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ftjyibej.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2hygmqiqm.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2zdwgudjv.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2cfcpakvs.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2dzczsgew.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2cfxhhwhy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ekricyep.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2evdzxtfo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2qwjvkxno.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2hlocivme.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2entfmuzd.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2bkozsfio.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2projfssf.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2buxwuqje.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2vphlwvhf.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ionytqdj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ggvqvwvk.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ktrbxhuy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2pqyzhjoi.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2llsiyzju.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2vcqqcchi.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2tiguwpbr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2wplsnvxo.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2kxxsvtch.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aekykwka.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2zcymnjwp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2jrqszdly.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pwofontc.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2arvyntur.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2seqbjrsd.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2vfnjycnu.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2glacrojy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2bfajhcks.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hjcistsi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2illmxiec.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2vckkclob.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2icsbtvej.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2mtcgangt.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2gjdauxbr.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2wzymyubz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2oqqzpzgh.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2jzujnsvl.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2potunsuj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2okfjwoxt.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2hrqdwmcc.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2qrrilptz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2iwtgfonw.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2yjykxyyh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2hrdpnjhu.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2odiszmzy.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2plbvvkkn.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ijvvxdge.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2asmbztgd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2xcmjpwss.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2bszbtcnp.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2xvcemtpg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2pjlmwumi.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2euglwpqi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2mpmhqkgc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ymzmfqig.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2nqttdtcw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2zorcloqf.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2nvdxpfvf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2fbgyghsv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gnxenple.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2lvpngaeg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2eexvphbq.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2cdlsvwjj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2izdvefmu.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2crkdahrj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2hzeqqrtx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2hyahvwtj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2xwqksfgc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2wikpddqf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2sawplflf.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2jydsnkig.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2kzeimzpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tcqzpwlw.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2cjppmkql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vxnfkpmt.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ftslstzh.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2luijtvir.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2zmspikvt.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ndlsmkqv.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2rwylvack.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2nlgvhkmq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ivjpyhqk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2vwzwldag.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2oqiadqok.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ikzxfpwe.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ftofbemq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2spnbumbb.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2echacybs.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2jicdkhjd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2aoxmhvfx.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2bbhcdafv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2foxebako.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2nmlghipn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2hmkoketw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2vyvmvfrp.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2dktjglog.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xeebtjbc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2psskijih.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ylhrthoi.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2qesteuju.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2yhcczedy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2awmbfgjy.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ddayyeyf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2salfwcpm.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2meminooh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2lgwaevtp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2lcwaiono.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2xydtopql.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2rsxagfaq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2isgebfga.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2cipswink.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2jzuiskmu.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2oxzvzoym.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2zwyvyoek.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2rrfsgrzz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wdykhcqg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2aqqhtyru.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ehyaedqp.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2sbuotffy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2unimnhac.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2nvoxauyr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2typfounf.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ikzgfici.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2sncdazwr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ezvcdzvy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2pwlqqjaa.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2lgwcuwry.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ispounpi.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2wzcmyscd.html


<!-- 参考信息 -->