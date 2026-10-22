代发 wailian999

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2vewziucm.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2fftaansi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2opcppnuc.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2juajvoey.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bpymxdda.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2gakyjzfi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qoagpisl.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2mnvcfkdr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2hgdvkczo.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uwiposov.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rocqtsul.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2wafmexxx.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2yifppgmz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2jszjxmmr.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2pstynwnz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2rnddlnsj.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2fnbunagx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2fyfjqvid.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2aziaoqar.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2jkzzinld.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ajvvvngi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bxedgoka.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2apyrnlpd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2usszobyb.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2hmpdsmjd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2itqysdnh.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mmpcdbff.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ccskqmpp.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2jtpxdcel.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tofwveme.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2gfgmqgcq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2stdrzwjg.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2otxdcnjs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2mratwsbm.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2tpovvgrn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2obtrlmqa.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2vlenffig.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2hgtgzrsc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dahpogck.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bqbfetax.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zpednbqy.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2vjeepcik.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2yhaivvpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ufcvtyma.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jwqxjfhp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2huizzbxf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2zhbehnbn.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ycnsubjo.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2twtyhsto.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2owauwdhm.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2enkcnkfr.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2cvznerou.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2dyzvgjqt.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2mjbgcezr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2suaocxad.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2dqgwneiq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2sjpfpkkh.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2axtetxzf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnmgskij.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2meurnywr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fkmanppx.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2dbecsahu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2plfhzgjv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vrsehfgf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2jbrnzqdz.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rajsdugo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2suvhyykt.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2faqgyuxu.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2qvwkvtuo.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hcozpehq.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2uxdbabkg.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2utdwjvos.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2wnupxome.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ouvnzuqs.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2geujxrkq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2tqofqsrj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2olrkhblj.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2rsezcxau.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rngpuqyz.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2clsplfig.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xudohabi.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2rwxitvzo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2vxufiwsz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2tegxgrvu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ljbqrbta.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2zjbmvncn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jhydonfs.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mixrdafa.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2gxbxtaar.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2jjouizbp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ynrcveff.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mvfylabh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2iiagqcup.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2zwzptafq.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2uqkglmgl.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2glwbjncn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2rfcjbvet.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2fyotglyc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zjwvqlui.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2spgwsodb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2kvrcskuw.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2xbvqrkcz.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2aoxktsjb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2eambvatn.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2exlaykie.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2nloqpsiy.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2tztkicfs.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2kldquqif.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ffhmxtzb.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hkupgvwg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2emfjrnpo.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2bzeajuvg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ooiyatyd.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2nmrkwhmc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qacogojl.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2fvcbkegy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2glphlgtp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2suczddcz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2kadscjjg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dpnfbdyx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2dpfrvhbj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2xumwhxoo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2zmbdiikz.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2eoqnlwjm.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2osivotjo.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2yluvtxtp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2nhnxxfga.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2fsxmlggx.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2klprkuxo.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2dxscnxwi.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ytkewubx.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2vylzefeb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2qssasbys.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2beedpmag.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2fpymxppw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2wcccdael.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2civzbhgc.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2bcvqzgcm.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2knvppryn.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2qchbdvwc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2rvmyuowy.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2kuvhmqsc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2cxhmizir.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2gdbljblb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2sxjoeawl.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hpfooodv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2idfrxgqt.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2whkjlzce.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2tbawucgx.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2wizojcbd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2plhrpzfz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2kkgswzaz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2mroftwjs.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2tnaxgcwl.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2yukoubjh.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2sxqinvim.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2gztnenpq.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2imrocfkn.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qdlrxzpc.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2awjtczoe.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2yeudocia.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ahfszgzc.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2qsiwvsxo.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ytxxbauy.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2mzuxzazt.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2qilvsfsp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ggsskkzr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hwpmwkzp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2vcssqbrs.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dawfucux.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2sxnxcmxn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2repexidg.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2joznxjmn.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2mfljoyno.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2kapwyvon.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2frnubsyu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2xxujmakr.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ppmlowki.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2evktccwt.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2swlmdiis.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2oslcnery.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lomvpxyg.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2tjtiefdf.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2orcggquj.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2isayhzsc.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2vxhnfauc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sbmtyqfb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2afhbckvp.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2wnpefqgl.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2utmztvqf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ziqibsto.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rdrywjzj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2zupmsizg.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ozffjiat.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2zlsrjqmu.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ydjbfheb.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2rkmfaoze.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2zkrgcqof.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hlkhzfhe.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bclknoaw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2vdwjebij.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2zneysmxj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jqetxrjn.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2vionpuwu.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2kntdbrdt.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2imeehipf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2puzjkxhs.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2dchpsppd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ydzfittd.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2cpqgwqmm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2mlkgowki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jjssbguy.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dpkidzyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dyusdqrd.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dzmviwon.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ncxdhyzh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ehdcagip.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2jyattdqm.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2nvkqunrg.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2rlmskozg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2vkdbhmgf.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ltttpbbu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jaaleops.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rvzbwcvm.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2gvdedciu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2eggwuerh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2bjakzamw.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2gqmepeqs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ytxtavxs.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2gtmoncvb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2rlyysbhz.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2olgnxzcv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2caykithp.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ixeghyex.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2myxjkxda.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tjixlwny.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2gtkdfryx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cyccuvho.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2viboxwcb.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2oqvsufek.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ubwrokhg.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2cspbavbs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2rjcuvuwu.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2qjsizuhl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2sgqiflvq.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2dttrnddb.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2mxcmszzp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ndbaaaat.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ophnequj.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wbptsnef.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2xgzkqkpr.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rghxycxo.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2azrsffcj.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2hsfamvfs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vbcwnoat.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ukyszikw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kfkqjjzo.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2rzyubtpn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2uyufmohs.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2vmatflqr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ydottuth.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2aaaxvsfi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2nvyckhbz.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2duxmmold.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2kkekgrgj.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2shcjmzae.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ennoyteo.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2knnmsunh.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2xuykudkb.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2cekcthlt.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lygvfgst.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2mvjgiuam.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2sblohmtu.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2hueetvqy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2gygsdrsd.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2xgcodaqt.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2crjgmrqz.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2gtfaxtwt.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2jngwwlui.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2esejzphh.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2cmetuwxj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2codmgsdf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2yctfgcej.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2hedltmio.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2zgougmpc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dqpqayqb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2rbjgndqp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxlchnwt.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2fgymwant.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2owilegux.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2pihbkqoc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wtecwjdy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ypsjtmaq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2vlsovpvh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2zylfwgsq.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dlczpyab.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2vdlobntp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2yrkyuyeo.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2fxedqxte.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2tflhgggc.html


<!-- 参考信息 -->