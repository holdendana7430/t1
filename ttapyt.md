代发 wailian999

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ykencwru.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2hmgypkyo.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2vcbftnep.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2abjmxrer.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2gpkikiql.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2etvlpsys.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2vutshzvr.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2uemuaxmr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2grdqdlef.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2hzgcriss.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2tiycuhzv.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2xumauypw.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ssqjpbhf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2clclerkt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2mztirqxg.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2hjefmirf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2hewropcc.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zpolyfmz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ykjmontt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2kashrtxl.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2sxtjmxot.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ljmzhwtt.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ozijtxck.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2fmzckulq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2nagoegip.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2qcpbaxhc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2kzerhgma.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2kfdylcbh.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2jslwzsvx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uksqgkhq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2xjwvctfa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yxnaniyt.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2rkjzpkxc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tnyyoify.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nnyxjgzr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mtlnxoju.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2yowpceba.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kwohgcjy.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2tpnkszgi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ibfkqkva.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2toeiwmzf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2udtymnds.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2fmupuvxk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2efwvdaez.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2rmmuqxao.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2zmbhyfqd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gzhoxpql.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2tamojdpx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2nxtixrbu.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2qajxpkbe.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2kjhbeltr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fmvzdzug.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2gzzzcmrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sxzscgoy.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ktmtlxpa.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2lmpzwkcv.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2cplpblbz.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2qehagcwh.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ybbsxgde.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2qiyauive.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2kpfwxhqp.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2khlhojws.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2syurtthl.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bvmpzcwf.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2zhrzfadd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2vthwotwk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvwoqmaa.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2disekkco.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2suyrrhuv.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ofdhyisa.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vaxecslj.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zjyyzqaz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yalqaabb.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qcdyusou.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2fblahrcu.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2apekunvp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2wrpemzsb.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dagdsdta.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lcnmgphk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2apfvbhrc.html

esac
来源：http://www.52xcode.cn/Article/details/gt2rohidhup.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2vywdnmly.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iingvsgx.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2qikduign.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jluzeiil.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2nkbgmwzu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2glzuyzzv.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uzwyokqw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2vtcrmafl.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2vbuvxqyf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2agujlsxl.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2jibwwfiw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2xqfqhjqv.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ugctpked.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tyqavqum.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bznydffx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2gjjblhed.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2yrccjcij.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2izgdchkv.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2unroujpd.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ecoezzrj.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2zfhnrewz.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2cjabjpuh.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2dvuuqvyk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2hsiptdsp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2bfievfzj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2rctgjzao.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2hrbpavmk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2vjnurghm.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2nfbilrcn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ihkzutcb.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2hntngnys.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ndfssjma.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2pmhkwqwq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2gijgqetp.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vptbiyed.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2tidycnou.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mfzrakms.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2wyzxtvek.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ttqazown.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aknjkdgd.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2mwkengzr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjenxsco.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2saewjude.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2hlzfbqux.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2jqpltaup.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2lsjnvnwb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2afwugqyw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2nftahuov.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2uqphencl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2tbpgzkal.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2akzonkiz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2fkphfuco.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2nmxnknag.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2zcwerndy.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2koizoapl.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2qqlqytdc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2xnmmfywr.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2luvrfrrf.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2phjwtznb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rpgdznrv.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2anjfylhq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qjlswqfv.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2iaqjajkg.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zsdqdiqk.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2mpgikqpl.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2sircwlxt.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2jhknoxod.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2bsfiyigy.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2alosalgh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2hzgxkrai.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2fxsxdlfb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cotxjfei.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2rdiivxgg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2eybureqi.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2zmndsigc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2wuescesb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ggqtyynw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2srxplgux.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2bfzualvw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2cutrcngw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2kfjangpc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ehvfegwr.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2fqrogzzj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2yecntcur.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2knycintl.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pxdaukst.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2mycpgpik.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2sagavpgy.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2skpvxece.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2eyyuxuvs.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2zlvapbac.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2mupghwnj.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2gbnaeofc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2lfvzavpo.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ljxzfnqj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2lekeymia.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fbeohjgr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2jhmqwvti.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2cscvigib.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2chwfsitn.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ahsnfkyq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2qibesbmt.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2nqrizvhz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2qovzgxsa.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2duuyksjp.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2zwnenxqz.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ssgzrxyq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2xmemnqrp.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2piwqzpvy.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2iulyivfc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2cjnmturl.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ybhrrwfj.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2netlwcof.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dbpswtxt.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2xgbebvsz.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2vvbbwdai.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2zolwycna.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2yeaweryr.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ydsiocld.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2fdqhrcbo.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2wlnojzhj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ewzocpuo.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2iayffcvg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2shmsnbho.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2tpmnltic.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yfucsfhw.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2eikvagmc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2fxukvjtm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2nqmcscar.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2cpriftuh.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2vninfvai.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2xtolhpkm.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2driwcvdw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2njflznyt.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2gnqrkcqb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2bzilwzxg.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2gdxaidgu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2nqniaoss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fpkagwhs.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2hdxjddgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vwroumhr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vhubpfum.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2zokkesyr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2oenedeqe.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2kgjgbfhi.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2dsuonixn.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2puwachms.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2iqjfdfiv.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2bogqdgtu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2eoaadsfn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2izbqicza.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2hnjrsxwn.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jrnxahlo.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2fxyyhwbl.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2kbqydskg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ezofhzjw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2xcnpiczx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2hxffsnxq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2duyxrquq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2sdzhbkni.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ctjoybkf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2uuuqlbni.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rjjmkegg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ykfphknn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gknwxfjh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2xwgdqeat.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2gpvmiwzr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2syrekjpt.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2pxipitqj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ntuedrjq.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vhqhvtrt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2hehsdjwj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2jkjauqoa.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2tzrgqywe.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2kosrojnu.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2scqhewvu.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ybhtpzvh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2itrotmhr.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2fasveyxw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ymhfkezy.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ajuyenwc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2mxeucvzf.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ggnurzha.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hazycquc.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2yximkdsb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ghjswfnl.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2apetywpu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2unuoeweq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2hapwqdut.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2hlxzlvrf.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2dmiquauj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2hadkzkmx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2itqbcxhk.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2vaibziym.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2wyxieydn.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2bkbltsmz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2pyxmzzsb.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dsxkfwmb.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2dmuaqqqp.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2fsvdhyea.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2drafzafu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2amqxqyko.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2jqoblich.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2oxkiypgb.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2osdmottv.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2hkhpwogn.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wiukdylt.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2kpgdadid.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ppjcmify.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2nxsbmgmv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2gcbphuka.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ieyvyrjo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lncmadsy.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2fvdwakso.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2nfixxomw.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2odvoyfyw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gtaxcmzh.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2xjqhevqc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kzkqnlpq.html


<!-- 参考信息 -->