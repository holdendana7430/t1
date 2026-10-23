代发 wailian999

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3dizyakvf.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3wihufvia.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3uvakjlng.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3jckihidd.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ilulrpsu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3lqxeyprf.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3uxvgxblr.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3mhafsmcu.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ndfhuest.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3onhbifxi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3dlnbzejl.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3bdbpatty.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3qaqbdurg.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3lkoplsze.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3pirwbruy.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3usgjbvmp.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dfeoguar.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3mqildnhp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3atpgzolh.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3lcvwauoj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3kaabxfqo.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jarxuzcn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ihgjvaar.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ttqrfsre.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3mokbbvso.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3rxwxferj.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3txjdljxa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3meknzind.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3mueaohaq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3yjvxvbvd.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3gpocqkgh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3zdlployf.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3kalmqdwp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vfkhxpcm.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3cwblrfdj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rqsmdhmv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3gwfyifqa.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ciocoady.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xiuublro.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zpyrusxs.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3qczrxsuw.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yfegggdh.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3wvozywvc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ncpgmtsk.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3uisskxau.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3iogxzrfu.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3sacrpatc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3nzgeswzt.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3itiopmuv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3qcokvczg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jrdxwgmn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3keubhyjv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3zzwkgzpo.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3vzwlghnf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3dibviaeg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3npowhyke.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3kixooslm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dtxfprea.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3glbwdgxt.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3syrgrlyp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3kahmgeil.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3mlbnlhbg.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3bxzgwytd.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3hxgbpybi.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3pzsejpyz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3gedzbktd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3qpopylkw.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3pzmtamoi.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3lokjpxvt.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3oojkhiie.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfzheuor.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3naalaubi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ecfdhhje.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3sefqluze.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dwlcncyj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qrujijsy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tqvdklrw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qnurysyd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nmxkcewu.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3jxxntiwg.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3elnemevr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jmlbwoel.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dwczdemd.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dukqnzcp.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3quzsnhus.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3snttkgzr.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3yvxperqs.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3kgtrnzpj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pomhnsst.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3jhrzjucv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fbfzmclr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xkvacqsi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xipbcfpy.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3dhotsmzd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qzbbqqor.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3sszsggqg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hxubnwjg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ggatrxyf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3evxzizup.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3lrdgtbtw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xrnyzoxl.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3fyxpvhdz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rqfudhia.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zckuiiyx.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3qbzcwdez.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3apuhxsmj.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3jvluswnw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3rfsxubnt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3htjutnoi.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zcdptsba.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zqvpbwyq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3mvjkmafe.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ypzrkgwq.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ggxdqrhk.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3phoehlmu.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3bedtlbbm.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3hmsenlsb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3khvyzxxx.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3rkzwppig.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3hqrhofbh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3qpvrzbzz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rttwnqka.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3milgyiwn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3nubkfrdm.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3umaliyzr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3civsrzke.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfeyemog.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3zetbkdad.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3zvfnunkl.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ebtoaroj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3uxgtygfs.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ksoiehyd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3kymswvcq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ujwwrqww.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3wtxwzwqy.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3wrcbnghl.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3vjmxthwk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3teekdfbi.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3vbvqyqlr.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ateplhsw.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3civahazn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3jtrhggfs.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3hwhttavb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3mprujpei.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3bnrvbojl.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3lkzggfos.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qnuectui.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3pazkxotn.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ktmwzezp.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3fxlznrik.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3kgyuomjc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3jaaifxka.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3lxoodnhm.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3iehzrtbd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3kjvfxpya.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3eqtofxdn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nfgzxsbm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3yxxpadsi.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3csxaeouu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3aghvzqer.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ohvwdhaf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3eicjmktu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3egsqnnfj.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3pmduqbsb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3uycabnng.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3pnnqrhgi.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3tzugnfej.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3xbmieftb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3gbxlegai.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3igbfchlc.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jttycuzk.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3qbukjesv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3mkqmfgzp.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3afxsadct.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3pgxumgcx.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3qsufjfkm.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3gyfqbwhb.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3adtlrvhj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3dnyfqbxi.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lzrxaniw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3mplfzthg.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xzzbyqji.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3xwmrmqnu.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3wjnyawyd.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3wgnakert.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3jvqpqudy.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3gsysilhn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3xcseatnr.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3gkuvjpzz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3afbiqzad.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3vfebljea.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3rztctyew.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3nwfvjlmy.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3tyrgitsq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3oerayjns.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3idnaydyd.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3xauuvccl.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3wzadzgzh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3szytzyry.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3oiwwbrjy.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3cuhtrqkm.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3kuwsxbml.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3cxxmfzdh.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lwnacope.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3wbbivdzr.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3wwobxjha.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3lyoeuyzf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3hpvtbblk.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3bnvxxyxm.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3fxjxderk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dezswymg.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jlltjjyi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3uwyoxiud.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ejalbqdg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zhafcekt.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3rnnwusdj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3eyloszcu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3mcqusaiz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3cwkdindm.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3vhwpinof.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3zfkwmlxo.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3qhrqxgpo.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3mdfnlrar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fppbiume.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3jtekplun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3peaoidru.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ekovvrqh.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3wyikjxav.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ilceyqxk.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3qqhwyrpb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3lrmcnxwe.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3atyddxrl.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3djfdhqgu.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ylegksny.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3obafnvud.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ojgdealr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3inxdpfnk.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ebbgajmg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3mpnuwkux.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3zhyqzqvj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3hozbyjng.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3qiwawsmb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3pymnkshz.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3xzymthcy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3raecijgj.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3vubhfegl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3vnrmevix.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hccgcsgc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3iryevohr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3toxsbmzv.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3raopooxx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3bzmtuljw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3hwatfroh.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3hargbbke.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3dfwhusfo.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fcpadmfw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3itcosixg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3knguqbis.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3xsghcgvg.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3brhtxzsm.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mbuhjnwu.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3knfdrlyi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3jmoabdor.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ifcppeli.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3rtvibwwb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3fnewncny.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3mdfjgoum.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3qaixkofi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3loswvylh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3rteatogb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ukoxdnlh.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3axjglyfs.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3rwqrqdkm.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3txlhqbkw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3gnufyiml.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3xlippnkj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3blgnqomq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kyzfjbyk.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3zgexscfq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ozihyxhh.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3bmrcxigv.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ulehswxp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qlhxkppx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ijzgzoma.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ftpifkya.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3dncctpuq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3dqctxymm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3jiexzuoc.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3nkrnjywa.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3hfkqzqjz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3pgvhetgz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3klxgalot.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3frslxrca.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgqrqneg.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zbksrzno.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ihfhdpur.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3jsqgskoj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3lmzuxfjv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3jqzrtllj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3edfbqkhc.html


<!-- 参考信息 -->