代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xgjmzruy.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3euvakvcu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zktwhkcd.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3iypdslpp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hethajbh.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3qmwnwzsw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3xrhblyzy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mdhjvscp.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3jbzlwpkb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3owurcpff.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3eribzmcs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xgyghvwe.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3prqktkvl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3tnydtxhk.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3hkmjyxeb.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3mwcvhnzf.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3hholnqmu.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3inmvsemb.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3swmvodus.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3fpybvvif.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3vwgsaiej.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3rzkomhms.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3rzjtxnvx.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3piutxhtm.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ywuppypr.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3libyvmke.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3znayvshi.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3nfjjoncb.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3kewmalde.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3mhuibtpi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3qwpcvqnh.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3rkieiwox.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tuyyvqnj.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3xdeeiigc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3skanwcxa.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3jwpcidcu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3awmhrwwi.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3joyeiqur.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3aoitxegt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ahqmxpqr.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3mwxlqmxg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3wzzmjiyv.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ymbpusgw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3qrmvzbgk.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3okfelvnk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ioqjvhtx.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3mknhlysr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3klvysupl.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3hyjiptti.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3afjhwjfa.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3cdwosnvn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ifvztaqa.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3dymnmhgd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tewyskey.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xxrjjanc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ynwoqeqw.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3xvzhwgum.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pryjiqgb.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3phtmkyex.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3zxucwsuz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ftidgene.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3vknumnez.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3clismcpk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3pqbrizwk.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3wjqqwwpu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3uyqfxvsk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3teppxqzu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zjkqhcam.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3myjdnlai.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3tuzzbdun.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3whrgnjlh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hpxngxza.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3xbizdzjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bzqiiurb.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3vcxxvptc.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3mbnfkqgi.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ajncdwic.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3zygwwwka.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3qyjnjdgq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3kynnvriu.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3pgolgkdl.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3hhxwwhbi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ckgvuvir.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3twblqqgi.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3guozvrkm.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3sghmenno.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjxqehnk.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ezdvsyuv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3evstoyem.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dkdfnfts.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jxxkpdeq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3abmmfadh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3veqeufll.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3alxntcip.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ejifjrrl.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3tqryxwsg.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3bfmkfkzq.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3nruvfpfh.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3xdpchmhz.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3eqrmvlpo.html

esac
来源：http://www.52xcode.cn/Article/details/gt3uspmynxs.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3zdgkseda.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wwxyntie.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qjbyqgeo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ablscdei.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3uwhnctop.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3acjenzbm.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pczhvvag.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3pwqjrqbi.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ircijewf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3oihbabue.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3bgywcrqc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3zjcgcefp.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3bsvdfwky.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3aemsfoaj.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dbfmfkqd.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pgcztfiz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3yktlpviy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3uguntchq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gzwhqsdy.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3nkkslfwh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3xfsmdmmp.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3neaxxphp.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3syzuqwwr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3bsljobsa.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3shghfrmy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ltydtrst.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3daxxlowa.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3xtmqrrtg.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3fwpcpbyi.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3htlnjpbn.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3zuuwrgrl.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3uzzypbgk.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3cfhqbnrk.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3wiyjrdfn.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3enegglxg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3xgucebil.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3kyuwxpit.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3njzcpjki.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ssstvqmh.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qanfsalg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3uxvxdqfs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3undeopqt.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3imiwbiqk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3dcydjqyp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3xhfontwg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3kqarwlta.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3pvyhebxy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3zkzzpqkx.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3nohvsokj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3zitfgids.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3xjeaasmr.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3tzxpuvlj.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3kukiiavm.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3anongwae.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3tfwabnlr.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wthfapcx.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3idvczsyg.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3gkgkrhwd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3blypvakh.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ithwwwvp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3xxdoiplw.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3siilxxrk.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3aymrtagu.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kfsdrkia.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3pdzxjvdz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kqbjpmjh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3xiokbwoc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3jktlsohg.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3lhxnonyl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3rubmxigy.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3htzeeksn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3yawzxjrn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ucqebsfv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3chwgznvf.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ddvkyibj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3sbkgqlhy.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3lawlcwkp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vtowrmyd.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3lvpifoaw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3svfoterm.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3appqacsd.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3fnyhulhr.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3wbmxidzu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3flsmqhhg.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3bfsrlqzb.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ebdczqqw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3zlzwrnzp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3fsweayeg.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mgfvrpzl.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3zosbdqzr.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3tafusgpb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3lkxcmmfn.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3cfbtjmkm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3jpwlpicz.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3fafvtytk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3rxccfsri.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ixqaoaqv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3xawftrjr.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3fhvwsbrg.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3acpevrwm.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3hupcmzst.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3nkwlnbhc.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3juhzldcz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3aanxgmer.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ftmwaspy.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3zkjixixm.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3xdmaddzw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3cnbootyk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3rfyexihb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ckuigzwl.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3adlucgkd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3fdhnlxog.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ntxndqfw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3awctqkcf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3vxufmsyr.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3otthoioa.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3edexdbra.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3dowkhbql.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nfwcaxso.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ytfqfezx.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3mjhtkcpi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3xthymvfv.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3cqfszjlv.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3qxmdbdpe.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3sukztsgb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xztfwqgv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3gujokjks.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3qwgxltcs.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3tvkgrcvh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3enpbjijn.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3dzerdjto.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3dsogmgye.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ocxzaojy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3dmhuwrtx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3mfqufnav.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3wkrdxpkh.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3fvxlkjjq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3lkjajhrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wqzfmrbt.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3akpwhngx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qpbolriy.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hhkwuhnq.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3grujbzgk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3sohymvsp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3crmuavaf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3xqzzqfga.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3wynwleci.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3lsjmfeyr.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3nggyffnz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wypggszz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3kucndbsy.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wjidyyzc.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rtxqxbiq.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3afrphgpk.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3slgalqto.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3nrzrybrd.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3tulysrav.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3btxmkrml.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3yjjkwamj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3xtetpwyh.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3qjcifdpv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3inzmvlxf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3isdbejpn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3uvxqacti.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3sfikfugo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3wmnvxrki.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3lkczjmnr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vvmpdfet.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3edziyrpq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3axemotbx.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3wtgetlfg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3qbjrpzcw.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3tphtfyqc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3bnaapkkv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3xiplftib.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3qmwszggp.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3llhplczy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3znipknnk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3uilqnxps.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3bhhoulmf.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3myjzajds.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3umpfyhvv.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3lzokhwvf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3dgzsvanv.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3fvkpurbc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3dowwihhz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vgxedtkg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3bossdaon.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3hxkqnpho.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3xfvlnbsu.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3rsauylpp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3btsuggey.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3zpqgyldr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3bvzpxhvi.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3yraekrlu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3vdfsnmul.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3kjmdicfj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sehguejh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3aabjwtdh.html


<!-- 参考信息 -->