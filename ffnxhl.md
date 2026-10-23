代发 wailian999

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xcsbziov.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3yntzvhnd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3cnlxvgka.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3zjcixtti.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ozmfywnq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lahcihrl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wsisvcil.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3gcdwwmjj.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ggqhleog.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ejqvzpaq.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3yichibnb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3dzhhretw.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3hpenlszm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3zinhpiey.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3woiksnye.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3milpqxer.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3tqhqaecp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lrnceoad.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3rilcgrpc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3khdmwrbp.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3mlygmyll.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3niqdupts.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bwanynuq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nljaackh.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3dnyygkqz.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3olzqexqa.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3tbsfxugr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3gohweejm.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ygmykjiu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3vhmmhpcm.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3lnbehnsq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3dqpawcxk.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3eoltbklm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3qufdmlyy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mvuueytf.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3phokuwkl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3lkcvhgib.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3nljsoaog.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3vtdmvmlb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tyfshfhy.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3fhucttlf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jfysbnjz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3idthubls.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3htcqzbug.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3wlnoqxfx.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3xdpugqhf.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3scghulsr.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3yvhoqlbp.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3futpzone.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3hyrjzgfv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3qwaywmvn.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3hzsslmqk.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3gokzqhpc.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3vxmuhgps.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pxogtysq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3nqwiycdg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ipvchqrt.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ikioxjqe.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3obdtxhfi.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3njhyxybu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gazzztyu.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3hjhdkejv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xoqdzfvt.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ollunksq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ibdoqyjn.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kojphgxn.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ozjouupq.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xbpmudca.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3ivqrutzs.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3obbsygmy.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3vnkslzuh.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3vkfnfdxa.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3uqkgtufc.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3lzkifvnb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pulbxadg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mzburwuz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uqdynesn.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3rcjomhjy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3holajgph.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3gnogmcgw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ilvueqpf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3yagosgey.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3itzetiyl.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3szpoyodq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wqbwului.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3qfryumyg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3khjfbhjh.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3snkinwdq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3wjzxfzdz.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3hvslzxtc.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3eeporxyg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3nalnduya.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3rchwzanf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hedbjnxi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3xhhwuhvg.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3atjnpoed.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3lctuencf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3wvphzurg.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3bkatwubh.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3mxflozck.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3rytekdyc.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ejaqeuhl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3lmudqijt.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3zrqkgrsu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3qbkzyyeq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qpvcqxlp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3plexwhyv.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3efnzocfs.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytwrhkaq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3tiryilkr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3snihmxoh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ygambvsx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3euiuqads.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3mblqbkpw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3whwqjcjn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3tqnoxzpz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3pplihpua.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3hwdnwkqg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3zfkfmggk.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3vadkoaot.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3hsvvtqjn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3tcxqrfkf.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3jojlzbag.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3xwbqhzkw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3nhqmstpy.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3bdlqqbba.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3qsdkwpta.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3hnyubtis.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3funehvow.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3vsdnpndr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3drrprsaw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3slgmkekx.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3dqvdeobk.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3eejzvwwo.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ltfvjhkk.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3rlorgqcj.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3dubllgec.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3piepkrrm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3hbhpxfjg.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3eounstvg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3sbuzonjg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3bolhlhsp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qzqlbewr.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3neyvbcpg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3zhmgdqvb.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3wgfebphe.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qiiebooo.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3liyvmadl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3tsokgwyf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3mqivkqis.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3gdvlqmez.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3uffcizwn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3mnanwsus.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3wppmgbux.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rryhribf.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3pmrjwskr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3xvpxprms.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fpsbtdpx.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ehnixiay.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3odwrfuyn.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3qcqvvfld.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3dhmaedxh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3svferoiv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zalchput.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ctbtpmnc.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ebciekvm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3qefhqhhq.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3seqajnsl.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3einnmroy.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3tsnhmtgg.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3tgszdjyb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3rbipxgns.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3qzdgnpkz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3sewhcxli.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3zbextcis.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ewrqcvkv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3kceyiszs.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3kexbnsye.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3sjylokyq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3yrljwptx.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3gqobeavo.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ovhycaju.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3cnipupln.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3whdutxlv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3mpzffdns.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3isbecpox.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3gxhfxgse.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3cuabrzte.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3bnosocqj.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ammfkuwf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ltzmbihf.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3rglchlvs.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3lsbibooy.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3qfyvgllw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ovckffxb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hssviqec.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3xizzakhk.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3xutaicng.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3zxuqgovf.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3aykwkftl.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3hxpqcuvg.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3glgvumtj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3vzetpbwm.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3vlnodkvp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3rtpvdasn.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3jssslxdx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3nrioyhzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3btqxkhal.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xzgqyjpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zcdvnqir.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ycltgouj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3trjpxjat.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdiuqnji.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3dlhhfuys.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3llgfqzna.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3oinuzjhp.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3vgvgkkhf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3rshaenjr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dcwaxtqk.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kirzaoez.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3igfosick.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ukasvnez.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3hvmfnxgn.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3cyrkbgyq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3kszdqxut.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3csvfscta.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3cuxxxmnu.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ooosmkdi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3yrgqieql.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ekmjlngz.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3dpokqxsh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vcbtgfef.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3evvagyak.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3tidkvohb.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nwqxteif.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3sgplcgdv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wczudmna.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ynyrecsi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ugpvvszo.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3pyxxjioi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3urwgdamj.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3hjmqdbau.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3oewbjnjs.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3rhpetixc.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3epmgkirf.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3phtjisau.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3olpdnnyx.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nqvtkrhp.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3lpfyfhry.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3rlcwpwhu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3azmcccnn.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3dzmdnger.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ntzrnmvt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3syrkrxwr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3rzsxwvqq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3kyimfejv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ptioaucv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3savwiazp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3pvaqymfc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3clvneilb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3odudqtgx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3krczbdzf.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ihrjorqr.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3jblsbpqu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3suggytmb.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3fhsroxfc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qjvytcso.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3gdylratx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3zdqgpfez.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3thqewbxm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3oftbnjth.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3gwdbwpwr.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wpoqvfyk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3phidytnn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3mowzszht.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zjzvmvrg.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3dxrahtnt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3zzhotmbq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3kjmrvrpa.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3lnpodynf.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3prwzfnwl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vgxsjpbl.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3yhmrlqde.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3eulyvhuw.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3vgknyfyw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ykkhhcym.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ngjbnqst.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rvmcdsdq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3hnxfkfhq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bkgonszj.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3luqshbgx.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3jgxbildr.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3rbgainev.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3panxzmxh.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3uzaqqbej.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ibmkjdxg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fcpamdpl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3xwpzjovj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3kbpvwyzl.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3fifnglwu.html


<!-- 参考信息 -->