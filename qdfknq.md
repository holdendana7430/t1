代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ujjrqnav.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3rjtwuxmm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3pfmyyyjp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uyjfajhn.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3pkflpbbi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lywybdcp.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ddiodxzw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vizaewvp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3rcuspffv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ugjxsbom.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3zcdvjegw.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3tzhhztsm.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3kjqcflgr.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ievaonwd.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3zdaldqem.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3eoatytnp.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3atlvxnlr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3aorltsxa.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3hhhcjrhf.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ijwqdohk.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3wclfaegq.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3hzqegwpy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3vokhdnwv.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3eavxruse.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3rvksjlsa.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3natkolbq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3jptdjmfa.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3krisjuhc.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tjleuyag.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3nfhavrnc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3rpcpotno.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3wrcdvrdl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3pcsppefm.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ibgxfpws.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dnyqjezw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3bljeccch.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3skmfvfdj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3vjvikgep.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3zfayxfin.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3kcdpekuo.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3jreqmdbr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3wbmtcoow.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ixxcrcbs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3zpwqotrh.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3oufnkcfn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kydtejpo.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3nvzemhdm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3acwzkhby.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3scgncxln.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ugzqxakj.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vmpfdnwq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hdrtjwbk.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ncdrijbn.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yccejmow.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3jehcywnv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3itliocmf.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ftjaltvm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3acliymak.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3mhfyeekl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3fsmrjpva.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3yckobyeo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3tsxdjrih.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3snurymcp.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wkphbcjh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3dswrtzgw.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3vsewwimp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3nhzxkhju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wmlehsaj.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3kfwsghhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3euxnkdcu.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3yrusftpz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3kjlsrhsp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3cttneikl.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ljmrvemj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3tehxfmxd.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3hjlakdrc.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3dnmcuier.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3uzzuuemp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3arcohnph.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3makwfavo.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3mdpaxiol.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mvvslqgx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdubyrwc.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3zggpasvj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3xglyswyr.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xtzqzdaf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3drvhyscj.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3orwnkyjb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3rnyfqojl.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3znnzdqus.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vlzpyxzr.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3cfbhisqf.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3vjkzkzvf.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3myxejndc.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jugdxzhv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dbufnhfl.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3xqpwmyrb.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3rhddwurv.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cvdncbgt.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ulpsvukd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3emezqatf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3jtebezyd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vjmcardi.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zqhwaods.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3xbxsumfz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3htatqfqr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ctslcsmc.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3qwrhnuqu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3zhtgvonj.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3plyxvkbf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3bkvanwsn.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ricedpdv.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ykywjnab.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3eygaxasw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3eeupismo.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mxdqiuzq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3fpewmwjp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3opplxpbq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3lxuynrrn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3zdxjagrc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3nwyfephq.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pacfdqto.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3sdtbpeiy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3jmxbtodn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3xyxtaarz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3igblrdoi.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ipqjcaqs.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3jgicvnaf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3btncfcul.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3bgkmfxut.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3touypwog.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3lypxzopf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3nmkjwass.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3lzdkqgsj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3tjfxbfzd.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3jvwcazfv.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3gbgonvle.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3qapespos.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dyejkguo.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3jtcvvmxk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3wecufwlu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3djetxadv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3rbldafei.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3vzwuyvqz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3jvorcspg.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3bjswipah.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3vlwlgcbs.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3wlksuzhc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3mcuujsur.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3puhjvpze.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3bzespvjn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3kxxemkji.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3zskytpih.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3fjpgqylp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3xufoppbq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ffuuojgp.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3whmihsab.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ntwuxlic.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qcpngcua.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ajbsvsxg.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3phzsylub.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3pixeqxcm.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3uknpgjwl.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3xugttnkg.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3pnksoccj.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3vylybmad.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3kforyzeu.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3zjyaytnb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ianaeias.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3epcxtyke.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jwcusrus.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ccsquzpj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3qseouygi.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3qjhctube.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jusbgmxb.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3cfacxwzp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3mhglkjmj.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3cggqfjqk.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3vlxnmlau.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3eycuudzo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3nyozabjv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3avakfigd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rnoikqvw.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ibuzfgzg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3otekohly.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3fyaqelne.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3hpszbkgp.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3xwuddpki.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3efheduzf.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3geeoaebg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3hjaizejy.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qlongnzg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3zhmwyzmc.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bfegclje.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3tdzvuyxd.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3mkvymbwg.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3iqrfgnuv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3hvljckde.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ptskojiq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3vrtmccnu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3tttgspiq.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3idxjpghc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3cnonloka.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3szyjoxed.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3wfktayyw.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3samvjxau.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3qzjgtolx.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3dogczqud.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ehnboaif.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3aeeivlkx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xwhbycth.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3pfstrkwv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3nvcodwku.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3vbfpdjya.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3kjnjtbig.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wyqboyvq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ifapvqre.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3kxxvggzy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3jepiktus.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3vouzuthr.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3fmhiiyta.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3jlwvfifs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ibyqwbjb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jlblaton.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3atrrrcmv.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3uhpuczae.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3bgjzxllp.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ovkfvwuz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3otdqjzhn.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3vcswqhmj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3howdgcei.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3dhustnng.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3cayglpkw.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3bbkklumy.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3xwuthioy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xwpnjika.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rlbwpxcq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aavqhjdw.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mhwguxdb.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3yhjtigai.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3lteutxlt.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3kwjwvxia.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3mtbutsal.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3zqmufygp.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3eoikmeqd.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3twrtfdbh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3npcoeeml.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dmnlsgsv.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3obrdzjef.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xqmyixiq.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3eipbnvrb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3acegkgab.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3oyreqkvu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3vgtgadyk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3oxlpfgfa.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3tcnuneai.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ewmchsvw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3huczhuaf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3plwfdywr.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yncewuqh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3selpbydy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zrozpyfg.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vgjerjuy.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3dcbudssq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3antuyvxw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ejlaayna.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3xfrwddtm.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ltytkvyk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3mpdymkrt.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3hgjrobpd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3azfkkvnw.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3fcsjkjaz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3pxgyuhyl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wncxkmvu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3vstbwxvs.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3akxagtxs.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3llluqkkj.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3bathldae.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3oxxoctfb.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3plquuwjr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gckwnyoo.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3xzjqucuz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ttpagxip.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3qceoijln.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3pixuxsoo.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3bdgixprt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3wyjkndgv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3wgqpvehx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3okovjfqw.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3irzvkqxm.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3zqkzndgr.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3tmakpdbb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3rcpwetut.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3wijndvik.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dfcvatwv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3xcrpqtvz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3oxydkndz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3urelomqm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3jecfsfiw.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3srhaqmwm.html


<!-- 参考信息 -->