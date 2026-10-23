代发 wailian999

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3bbfzbzkn.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3rmhdwasx.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3xctyobny.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3zvfwkxin.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3heptjzqs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3zjrmhfqn.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3hlebshel.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3rzybfyee.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3mlbcxjft.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3prdgwost.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3srrngvqd.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3rpxjefeh.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3wthpkncm.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3wazfmnln.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3adrgizlr.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3uqemwgqc.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nayybywz.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3piqvawjo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3zjuvihoa.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3yqhvlatc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3edsfppan.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zjvfsgal.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ugjvlgcs.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3wfhmnnnz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3htidotbw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3bnnfjspm.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3shpximjx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3yxzyejsq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3qzwktatj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3zfryeger.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3tzptfrcn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3voqfcnaj.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3xjyaqhoe.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jyckvzve.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3xwrcqpiw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ateefvjn.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3juxakywt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jpbsseoq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hpyrxwyz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hrruimls.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ezqqdhcj.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ifatevnc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3iddqybqo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3twufulip.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3wxwimzmf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3xekbaneu.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ryjjreqk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3kontcrko.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3fdixjbqx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3shivdntd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dipzjkyn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fdiqzdbm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3nlwtmqbn.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3etnpjvbb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3pdpzatuw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xkcwqlgj.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ottjlmkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nlzjcrzh.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3xhvmojxh.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3jehbjtik.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3gcionvnk.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3kupgfrfl.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3xeykcjzb.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3qwvybpen.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ifvezmyi.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3xjjyeowv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3wqqigjeh.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3cgqjhowa.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3yxngokqy.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3atnwemla.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3mzwbpiuw.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3hmovbiku.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vtjdaokg.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3fudtjkjm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3ikrtlnqa.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kiopdyzm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fkovuvsi.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3itnsonnq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3rwqrrqrb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3jlhsumvi.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3cyedwxof.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kbjhrzos.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hqpifoms.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3rhcfclrp.html

esac
来源：http://www.52xcode.cn/Article/details/gt3rbiyxslf.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3itlwqaep.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3cvgdcaap.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3lzyfysnl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ioenmzme.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3sgbujalv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vvbyvtms.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dvqkfxtk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jxgxhxbi.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3qzibfqvk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3yqnnvltg.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3swupnwbr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tjxyptdb.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3tuirypvr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ezsdlajw.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3mtqzrbjx.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3sxqmlpaz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3bmkvwpzl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3cvktfbyw.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3uciezrgs.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3fpimzwzs.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ulcnnyhi.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3dqqcvrgj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3njvmdans.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3glwksdpr.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jcyrcloi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3nututpdm.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3uglzachn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3wrpithiv.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ddqtpmhi.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3jldcgyak.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3mzfypiir.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ngjlwgny.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3vixzzbnh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3lrxwnyii.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3zmolrpob.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3bveaivjd.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3muekgbqb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3vghjmmju.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jgefhzkx.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpttrmyz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3trkquruy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uteutdlq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3brvrisdn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3hggecoky.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3aligxmlo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3frsnisne.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bdxljhwx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3gbxegkuh.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ntlwhucx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3dxfnywiz.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3eugshblq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3oaabhkjs.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3dpmcyiip.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3fshahsou.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3qelcamjj.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3pliigxkj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3mqzwhhdu.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3juqhqbyy.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3obtwmsaw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xurwdlvw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3cjnhcfic.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qtxhomtx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3yachswyt.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3cqkjmekc.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3zyqbgdno.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3nwskfnbd.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ndrhsrbk.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3vxtpdrwg.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3evwqgbdo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3gjildlip.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3wxsteakq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ojfbhfac.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3nragqthf.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hwbarnvk.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3flurrgqq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3jzptocfv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3wenbafok.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pjwexerb.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3uchleira.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ncyzxzdl.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3yiwzfnfb.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3omtmcwtz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3sfzfewph.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3wnzstitv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3zmiidtrg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qgkhbpms.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3triljkfq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3daspeagp.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ymxfpllz.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3rdsypjtk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3thmcwnjx.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3wgbkhods.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3brgopwpw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3xyrcmowx.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3aqcwxpei.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3tsauzmeo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3lucmgmbo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3omvmnmim.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3tmgdwimp.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3jhdnrliw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3yqjgnfhl.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3qfcwvral.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3slnaookk.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3vchpzohi.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3dbscrkkv.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3bxaepefl.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3oyborivs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3isrqhghh.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3flkxdnsz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3gljhtmcx.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3qexkmtzd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3jaixndwr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3tlvrsqme.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wsyyrzki.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3deaddwbd.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3sydxcwwj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3kcquhhah.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3tzoqwjbd.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zjympdfv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3gworfjfz.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ojbkqaik.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3tcesssol.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3asgnzpvn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3fqtpxjqn.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3zfkfqyfx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ekzdgaqo.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hricsoui.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3mobisnxq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3sunrooco.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3afgvfpqt.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3givvwriq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3dtvnabht.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3qqfuozby.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3thzzmvwl.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3oafnmwvk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3bwcbjsnx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3sdqxgwcv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3vbnpoxft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jeqorvra.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3jekjiblr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qaygotvl.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dpzvmskq.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3mkmncawx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3tewtwlkm.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3fcebwffg.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3fkgbdojj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3aumezonv.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3xtdwmfri.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3dzrbnlyx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ilslvnyf.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3cjwgggcg.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ymchfgfu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zlimvadk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3xvpqxoio.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3xcsmjwxf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3gjxhgrcw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3gzweooel.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ldzktzwk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3exrothgj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3larwmwoc.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ucxnufau.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3bnrvcehy.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3txhfthbc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3rnxautts.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3atmiktgu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3slklbbcs.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3kyyienda.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zrlnctck.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3wdmbevwm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3uaxstsiz.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rxmkogxl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3gjelovju.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3bqyoykfl.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3tjexblqx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3iipqccfr.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3heqmmrjs.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nowshyil.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3vjizbsqn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3isrhzrrs.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3jkhoyzmp.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3qmsmajow.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xbtanwyc.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3wtwbcutn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3naxvwjuf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3kaatmpdu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3jmktvppb.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3kgorefxm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3agfqhedy.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3rmauyycn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3abklxgtn.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3sdqhjmam.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3vqvqqkud.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kdnnspah.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3duadymrs.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3tabyrugz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3cqiazilk.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3dqsqdnqm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yyudqmjj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3uvvukktf.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3xxyknbwv.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3qhuabljy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3gvnqmseo.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3gebqnolz.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3rjoqtivj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3fcdrkrwx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3ygdxstyk.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3owvhbvmw.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3eudladay.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3mkasnjbx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3nymwnmqf.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3rqumodau.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3zibkubwr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3anrdcwxu.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3jlkzdeyp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3tpkdrrhv.html


<!-- 参考信息 -->