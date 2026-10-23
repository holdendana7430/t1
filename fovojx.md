代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3rspfpfeh.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lffhgvwu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3aboiltqq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3bepbydow.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3sqnnklkp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3hnvxzjhi.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3nslcycvk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3dhjkcace.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3hwepkfgf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3nfitzgvz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3pmudcvwh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3iagvfdmx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3dqztusmp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3avzycbzr.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3hkdusqiv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rkhqvttp.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ttfczibh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gufbyltb.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3fndqrgtl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fgebjvjv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3hqqfiprr.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3urdjzbkn.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ibevbobn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3kwhhjugy.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3asatvgep.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3lpcdnasa.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3cmaivxvu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3yfogqzwe.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3gnuscyvc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3urtngrws.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jrnforqm.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3slfmearx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3nncujwru.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3ekbptiln.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3xqxfhkbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rmfkzjmb.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ayutkqli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qqgxlczb.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3tovhouwe.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3bamfillb.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3odkylbkh.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3uokuzhwb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3hnpqzays.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3fexoncrb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3dkwlwzmb.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ilnnppyv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3eyfzfkkl.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3otzzmdhf.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3blkgcjak.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3oymwhvnu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3gdpzmejr.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3mudexdap.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3drnsivmo.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3jmdhczog.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sciudjdv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vqbhbfux.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3rhavaeue.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jksdahft.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3izqfetkr.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3wmfrpawy.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3iahwiodl.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3seaihckm.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ftfakatw.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3imbtsies.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3xybfgtwv.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3xwqlzmcr.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3vtnplsxl.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3cpcjeebn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3cbhfqmnq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3rbvqckac.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3navctpfk.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3obxxsnbv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rvylgovo.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3dzfumimy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3walllcod.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3mqvqannc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ygjdtwco.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3lgydmadg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ecqrfafw.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3noihgsjb.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3buekkpus.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3jtzcuoxo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fmzfibai.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dvdiqdim.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3lgwiuusu.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3krqdjmdq.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3lejmrnxf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gqfhnmlf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ojdyajiw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3apxcaykk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3eogozxqb.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3fnmoslui.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ersgasyq.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3gnsrxjyq.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3qwcozkoa.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3dnmttnhh.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3zyxvqcxb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3iavetkfc.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3cvqtaqcv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3mtlyeadi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3hzbxoprg.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nargnxmn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3kuhfggrf.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qkpuplea.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3nfhsgbfj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ihywwiyh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzxzvvtf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3wfruldyx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3tdescbdm.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3uawwonug.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3letzavxg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3rkvivmdb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3mmngyjij.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3phnvyyfa.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ghwpivpv.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3flacnbsa.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3tddrpbxr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3lwxabqbj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3mfkmjloy.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3jknttvol.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3yxcsehoe.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3kcrofhln.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3hswlejgj.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3qzbdblwk.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3nuxogbgw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3zkpakfib.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3dgghyriv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3vxrwdahc.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3cvnpmtjx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3mjrcooxr.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3djfqdcnu.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3bdkrlfiq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3zsvfpmaj.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3tlavysfx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3dqhltgst.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3aizbzvsf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jdptcxom.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hgtlujdr.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yeubvfgq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3thulbpwn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3vtfajuen.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3fjroqibo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qhvdausx.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3nuegznmv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3bkctsutl.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3jnbrzwcf.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3nnisbnzm.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3uphqcodb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3eaaeipqv.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3kmcpytpz.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3najulnsu.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3pmudgetx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3okpgioch.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rppooiih.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3lszcjnab.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3pfvyqier.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3zijvefmu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3nyqlysxr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3hhmtzjzm.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zrhnurtv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3wczhubxo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ipoxnggb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3tqusqmis.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3jyrmqzls.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3uxewhuqg.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3rpigltja.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3puzlyaes.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3cguuxozv.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3msarcfos.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3bkdxcfoq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3qenzsmhg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3kiyttwdl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3fqyfksaz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3kuoowcmu.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3iobixups.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3mbvularc.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3pfwxjweg.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3uapugdaj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mzqtbrdo.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3zccqtesv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3jyzlorhn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ghxldpjx.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3gbqigivg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3flucemqy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3uunuxxgj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3hrekeroy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3kvaadqgd.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ttcdaibz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ptekedyg.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3prtdefzv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nhfmsovp.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kvnszwms.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3oratrtms.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3pngzpilo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3lchiioxf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3tycwgedt.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3uydbjaev.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3dndugslw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3thcxpjis.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3yzyhvury.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3dcgkbwfx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3flsootgi.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3rwhoyrso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qaxfbfeh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3zsnfowjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mdngusoy.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rofsrshp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3bnjqlqbi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3npmepigj.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3vmqgbkff.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3fwcbfdba.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3apbojgxq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3uyjpmdpf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3vsamiftr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3jilmcgct.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ymnwrzls.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jjlvxidb.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jcauqujz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3dbafmzps.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3cfyycjht.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3darwaald.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3eqlroesa.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3eazoegsh.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3pxswtgjf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3vvjfahjg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3znjhcnza.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3hckbgrlo.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3idnterpk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3belaemrw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3iggjthxu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3oeqwqofw.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vimnpfcy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ezkbpkez.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3hbxelxno.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3gwrzcslh.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gbrsnjuk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3inivzpii.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qanpkcoc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ngnquqks.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3rlpjbxvs.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3epxxewji.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bhdmvobx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ivqeqwin.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3yudzlmog.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3mmemlmuy.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3wcttzihw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3piuokbqh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3wfigfqzq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3sxsnypzq.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3mfjsnysa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3oekqohil.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3twgruysx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3lcbdlozk.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3zfcyxknd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3smfsrmdf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3dezdpehd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3xlrikepq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pugmznfa.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3vwlwfaho.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ckkslmjl.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3uuoufzcm.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3zykifeax.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vvjhmxmp.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3frwlilxi.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3rohgbpwv.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3fkhjfpbs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ivelkdxf.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3vjxbcosq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rbktkagv.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3opbbaiul.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3pwaulqcm.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vgvrrxsw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3veniepjh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjuswmue.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3cppswzaj.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3dxlsgwrm.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3pgjbttoz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3mcumiqrm.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3oqjualnr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvuwfflw.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3xmnrqwwi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rsrcgaxq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3mihalgme.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3akesnmlc.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3wocjuitz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ivndsykj.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3scnlfpbu.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3nnvqcvui.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ykxfihwv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3rjlbtynx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ttqzodsg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ufayekxc.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3olaanobe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3upwcipwf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3jbadvltp.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3rhbfaipf.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3saevybjm.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qtffvctt.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3thqulbfb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3acazjxgc.html


<!-- 参考信息 -->