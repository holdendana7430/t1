代发 wailian999

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2qmygtzxg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2popfoxyq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2wupdlkxo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nciwegma.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2nuberoks.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ehqigxiv.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2mwzmsvxf.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ktgsahwg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2htelhpjt.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2cccsifqr.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2mrblugrb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2wvjvqrmd.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ufuqtnod.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2hfkxxgif.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2aotmptge.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2xarkddkl.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2fsksgejz.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2yfsicoyb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2mxythgpd.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2dsvxbvsc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2mpeuczay.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2eodcgvgl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2vxwdipnh.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2jgpgntih.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vhsxpzas.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2asjtscmt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ninzjgca.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2rxuqulmc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2zoskkjez.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pwozhith.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xyqnmmwe.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2omvhkdzx.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2tntjlorl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2usoxcfrs.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2esvzvxtt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2bkjvvvpa.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2nkdpzbzg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ncsozcba.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xlgmdepb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2tawwkaqk.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2scstbdtq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ncaotsme.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jqyxpmgm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rggmdvhu.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2olxhzeer.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tcxobgik.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ssxjhobe.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ayfytewi.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2rwaliqdk.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gzbtjcrb.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2nztbjfen.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2romsdzqf.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2rnnkafoj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2cvdjxqmx.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ghcxwjlv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ygwphcaj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2sgznxrwf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2zfnbginz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ndafmfmg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fogezqhx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2jbxccaqw.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2iydrpedi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2gxzecslg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2alajcpcz.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2wjonsqws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hmjfkybf.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2hzixmqwx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2hbynlilc.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2qhucajvc.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2vxiornnm.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2nwcjkzof.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2zuunijfj.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2lvjavgom.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2imznjlco.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2kawhmeoc.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2oqdwmjfy.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2xiizdbac.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ggohxsnk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcwabiun.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2rbcslakx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vbicoibr.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2sdkvibaf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2qotjfkuz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2cfhwycxk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2bwqrwwnh.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2grfwjjxa.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2qhijotkw.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ulgwgyfk.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2mtrwofgw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rnohizfa.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tkabuwqd.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2thyncigj.html

esac
来源：http://www.52xcode.cn/Article/details/gt2nuwuvprw.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2gjismrhs.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2abulzqif.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2cifwirah.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wwpnnaro.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2pbcsetkh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rtcfdajn.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cbkityqc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2fbtkhnyy.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2bwmplcaq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2kkjqtmja.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2lorjvqjv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2fqbcdnem.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2vxntoewq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2reyviznm.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ensfqfcs.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2eaarhekn.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2mfligeoh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rncbegjl.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vmkgdwon.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2nzbindig.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2splmlhds.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2getifdeg.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ccdgnnzj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2cdpzyggw.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ulcelpae.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2mpbenapo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2lakxcmyg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2kkwcwhiv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ehaqewkw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2bytrodph.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2lkvrhyeq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ldxdtqau.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2uwrtyngu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2igivedub.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2naqdfewg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2xmzfrnis.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2swtdbzht.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2hoxskcoc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ofxnieej.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ametiqsk.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2lxzqsalu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dadakdjy.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2yqjonlas.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2bstntvdb.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2lyfgjsny.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2kyncmndz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fehpisqo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ycfvdsby.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2vomhhtxi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2slfsqdoc.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2cdxxfmds.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2fnqaacxi.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ezyeeiif.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2osgdusaz.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2rjcvdmdg.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2iaqqmgde.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2tgetufiu.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ezqbyupk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2mtmnsdxp.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2untkitvl.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2glttsbde.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2gzvrkfrb.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2gytdugyj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2niglzegf.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2udobvaqm.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ujghuprp.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2qakpmvnj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2xjxeqytj.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2xdiuqjeu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2nfssxtab.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2innosbzx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ntnnmere.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bqiniyam.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zclxusuu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2vaubjwfq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2eftalinf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2pfvdkmqp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hydpqufy.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2cjdqweff.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2nisrnpay.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ovruamwk.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2viochbre.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2jwrbhhno.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2sldrydke.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2yssmmmkt.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uktlovbq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2otixennn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ylvrqmym.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ervnbltr.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2reaaepju.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2fjpxtvxj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2rcztoyrq.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2tqiynaxu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ixispjyv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qopuixiz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2xwyrnkuw.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tcxifvxi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2embwljie.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2iqdrqska.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2geliuxoh.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ffcsponu.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2uyzscust.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2kfsdhrdu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2wscyrjdd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2csyoyrzt.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ztqobycl.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ioyuaroh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2bkbwawyq.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2wuygykqp.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2iqstcgcx.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ggzavemr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2apwmiypa.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ebdfkbxl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ozhkqeka.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2xactfhnq.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2oxiknzvw.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2inemfvcr.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2tnsnsehh.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qqmpwrya.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2uqysjfdz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2zxseghqy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2opcjaprl.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2wgkqavfk.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2nduwiwev.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2bzyoitph.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2hvmlyogd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2wsmgoqvq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2yiqvuagb.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2wuxsyuwh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2glybtlnt.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2zrexcxnj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2rugluokf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2xenxhsnb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2iqxijzvn.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2qtsukorg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2xrvgdmrm.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2dusimpmv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2nssumarz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ozxfndda.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2pqhcavqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixmlcxbs.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vrrhgnrw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2dxsdaxlz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2wyvymsik.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2mwvofaxp.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2fiyzenne.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2cyluycln.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2hgkvsoms.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2cgcgrpyb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2aojixemo.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2akeoqixe.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2urzbgvel.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bgufykpi.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2kryzlpal.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ltjylial.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2hqwcmvsh.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2hbpviekm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2tusjeiwp.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2vuwwtgbk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2rirmbbom.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2tccfxxfl.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qyciqene.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pvohyjpy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2lqlngolm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2hpplsgjl.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2eqcfgwim.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jtsefcxa.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2jrgkluhz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2kccaoplt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ofgcczpu.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2gsszgrhw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2xoomjdkp.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2douvzbya.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2aqphcmsl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ttxkzkus.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wosfkyiy.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2onuzmfld.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2iudyjmkr.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ybhigwrp.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2vwildsda.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2boziwvhf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ogyworpx.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ptzzoonj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gsozjtzl.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2mpjajqmr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2hbcmlszo.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2fyomtejp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2epvcbeiv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2furfhltc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2nsoreaya.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2kxqaghdb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2tvbjyqmv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2isqsdnjb.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2tpaqzfiw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2kaqwthfu.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2hgoslwal.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2fvxgrscm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lmarnhyi.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2cxyzsadz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2lgxdmyvt.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2muhqvoxf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2uwqbwhuq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2vtdmgsgm.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ivvbzczd.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ikgocpic.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2psjxjqub.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dqbigqzg.html


<!-- 参考信息 -->