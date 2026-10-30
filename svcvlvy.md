代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/giilxeane.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gkhnfdkwa.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gxfyemcrj.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/glbiclgxh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghajbexop.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gtdoizwpo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gddxbctcy.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gwrosmgvj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/ggeskjbzw.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gdtzwlulp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gjvryzsdh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gewbpzlxo.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gdzgscevb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gzalpcpfy.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gpgzfrvod.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gnfuwfver.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/geczbhdun.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/glhsifzag.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gpngbyvxh.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gobdihweb.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gfqayftas.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gfsnqxwmz.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gbeygeggy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gptomesze.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gmixmjylw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/geizpglmf.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gfeprqtyp.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gpnnbczsh.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gdvzrmpix.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gxuumovpq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gnbevvxwa.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gvxpowbca.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/gccorsfmf.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gvwmlkcqu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gddlclyrt.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gyihvysre.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gavfnrkiv.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gmuzgsdkw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gsdlydtmq.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gkxizfaqv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gjzmofswf.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gkxergexs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/goilletvb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gvlcwmivh.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gcxivivpl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/ghfuthbfd.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gykmzkyff.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/glcjkxpab.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gqduolnyb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gtvufswaf.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gxhnqrejg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/gdonlgwtw.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gfukpwnps.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gfmxudfvp.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gmxgzfmkg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gtpqlozje.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gjgpuzxmj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/goxsukrwn.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gekikwopv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gtxbbutxx.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gkgvwzwcd.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gesxxsfyu.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/govkrtosn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gwfjnjord.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/gzfrtxoxk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gmrrfbcfr.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/guvlnoqwp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gqiejbosr.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gevmhgdio.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/ghgcbohvj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gieqpljmo.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gbabpkgtv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gjimhgunu.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gmwgwuvim.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gjjesdndg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbovgwjyv.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/grhtuxdaa.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqvrcgqjq.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/goyvbfpxa.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gwpmytngo.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/guqorbmhg.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gnwruhewp.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/ggnblyqwe.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gssormdgm.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gnqpcagul.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/geethbivl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gxofcvukj.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/giaqdtton.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gnkaysuxa.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gywariahv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gjfteexpg.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gvscjopkq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/geaamlopn.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gzesgbeos.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/gnzbneaig.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gyfxrohzh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gpvvyzpld.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gpgrhlaiy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gaubdnadc.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gfzsfwfgv.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/ggqxixbwa.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gfhlkolqi.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gdykibrqg.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gumauybdl.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/goscqkcpu.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gpwedsxqu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gzykxxijs.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/guhofswpi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/glqyfcesy.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gvhumxbka.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gutvwhgpc.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gdocxvpca.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gljxlhyrx.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/ggymgvdwl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/govhsgwgi.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gwefegwvj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gvudvpgks.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gskuahbif.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/gibmluayx.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gtlpcqncq.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gztbogzgy.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gpuhkwfdk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/grdtrsitn.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gwllvyavf.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gyrbdazbv.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gwezwkuia.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/ggxvuavqr.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gfnzheytl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gtxzevtjb.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/glvggxnav.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/ghfwzhrco.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/getrqajmz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gmqhstyxx.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/giykmfdmp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/grzhfgdpy.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gxxypbhgj.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gzrcnndmn.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gemcfzmku.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/grrpqyxqj.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gxajgzwsd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gtrxwyqms.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gpiuassdj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gidtzwyxc.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gauxwzrne.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gihbntowt.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gfropqtmw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/giiccscys.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/ggxwilpnx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gpbdjndbw.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gysfryplu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gpbxvtzqb.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gztrhlgvv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gvmpfkayk.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/ggcltanjx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/ggugoffxt.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gkpzffkpi.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/ghtweonlt.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gmbqifwjn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gxihbwcoa.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gpwqsuhir.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/grphckcku.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/ghdmdxkzn.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gydcymvzw.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gbexdpino.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gksgmazjx.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gdjoelgej.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gptpdqxnz.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gkwsyyqjm.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gdztgsknh.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gupkemazw.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gielqyzny.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gnqmwxtli.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gobhzacml.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gqndbzzkw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gyaabwyok.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gpgizpwck.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/grweyefry.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gtujuyyud.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gxusrimuw.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gxkissiyt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gflvhcziy.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/giarzpwrb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gdodkuyab.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gzytfmusd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gwqxzwcft.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/grsfljkum.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/grccyiciu.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gftaftfif.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gvvmwmqny.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gktcekggq.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gqgrrevcl.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/gxxkfzdwr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/gqfgblpjj.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gpzozggrc.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gjkbtqkpj.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gnrtwbcjs.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gzjksmdvq.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gmevxgcxl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gkfskkuoq.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gbaluqvib.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gokrkoddl.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gndrmtpat.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gesxzrxvc.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gcpezvgek.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gegfpihkb.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gvkcripfm.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gssshnrai.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/guxhkfymt.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gffhzikxc.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/ghhyzezml.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/geohrxoiy.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gpkfdycav.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gfdqhzdwm.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gnyuxduop.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gtafrgpif.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gyoykoygi.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gdrskjyia.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gmlrxyotz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gpogfvrdc.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gnyjlwvtv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gsbwsbnyt.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gskodyzxx.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gdswjddxo.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gcdqcxnsq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gizwbtoln.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/grpfkhnrh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gvvuldcak.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/ghfkfmehm.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/guaexmndn.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gdkzdwhby.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gupdjnmby.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gqxhgaxgs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gmwfklbzo.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gyyvawggc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gsmsjncra.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gafivhmpk.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gidgwbuyl.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gdihmebfu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gslmnfyxk.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gpbrrwyhd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/ggvyctcrf.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gdgzhmunf.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gfwtwnlpl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtomodgcj.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gsydhcozv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdxpahxsa.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gtabuymwl.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gktkyiabq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gduzqoher.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gbbvnrshj.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gewzapfbl.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gymzxkunt.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/grbbiumvh.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/guwtthfid.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gvinfrpsw.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gqlmarzli.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gcmgffjrr.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gbvlqqfyx.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gqcnssmos.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gzonltfgc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gavsgbgyx.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/georzlfxt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/ghesdubnr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gtblwpmnq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gdytmiszb.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gckgposnt.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gnlceospp.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gsnwdogro.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/ggtvnhxcq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/grkiogugm.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gqklplzew.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gozhbxuoq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gwrqylpdz.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gvqvgbzpn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gbfyfompe.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/gpgejjnsb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gmaqywnfc.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gqwwksunt.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gwbwznpts.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gvnhglpuw.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gsjmoownh.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gwzrvrrml.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gsjgrrisa.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gphkzojxl.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gbdwnmwjp.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gxljknyve.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gnatvfmwu.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gfhvjdikh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gzqczoiwd.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/garfjrusx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/glbunfgbg.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gzoihlajx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gudyjbkoh.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/geugchrac.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gyasnjbhf.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gzigasryn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gxxtajmeb.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gvsxdnzzv.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gzeqwzdjb.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gquzeheba.sHtML


<!-- 参考信息 -->