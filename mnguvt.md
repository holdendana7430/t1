代发 wailian999

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3rpwfxpai.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3tswtysqy.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vfssbiym.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3selrymcc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3mbtzjubw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vbenwlet.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gpealnio.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rcjbznyw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3kmenqsoh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fhxyelog.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ifliqxeq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kiqhfaom.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3qyumchyo.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vrcwwpuq.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3znuwzush.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3exvwfxmm.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3hkjdhsaz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3qqpzyhbz.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3hvuzoefy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3jsyjwrzf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ljmmcyzk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3dpilprlu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xqswqlqp.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3lhbvnyvk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ghfbywwv.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3ymfmojio.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3yqtnavxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3facpmfph.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3upetxwkv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ofzgzfbs.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3qjmhzkyp.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3vokirgoa.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3aqbagjyc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3muzrhljc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3dhdicewu.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3zjitobvk.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3zyigtlnb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3oiumemfh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3arnhnfvy.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3uffjdpnu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3jlbdmkru.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3pqkfbkmj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3hwgfnwih.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ihlnazsc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3yqzxtafl.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3zovhdqbl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3nlzaedjk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tqhskely.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3itwuwqiu.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3swfhuubo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fsdtjelq.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3idemukso.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3curynrfi.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3cvypwaar.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ibsxofha.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3zweybsnr.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3atcujafu.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3fwhynfpm.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3aztatfey.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ltdqegxi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3rgengwrc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3egkinpuj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3dudubbqg.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pougakht.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3drazluwx.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3kpmxoinz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3rdbkoubk.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3adnkmmzt.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hehkxeqj.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3qnuamdrl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3aojoxxkx.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3aorefqys.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ubewjabb.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3azyjyplv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lgcolnnd.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3srvwyupq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3bsmzqfwr.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3hayzqtsg.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3hdqdmuap.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3wrrbjzfd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3tggdqgpv.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hawfbcmu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3jprceber.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3kankyhbc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3xsnobdpo.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3tgpxwgnq.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3loebhaen.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3bnplghsm.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3xerexrfu.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3kfuukmzk.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3prhbmoon.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vddfwngy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3khdhpkap.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3oqorzhno.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3tyqeyano.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3hjiwzxof.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmnlovze.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3iqfnbetz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3cgdtmbub.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3zcxmoexk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3exxmzixv.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3keauhjvt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mqcmtdyb.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3jtrpvwzc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3vspjirwe.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3jbfbcygk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3degzsqum.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3fmvmgeuf.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3tuudafxm.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3uvrviahc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ovqzogsk.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3vrnebeou.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3cykqebxm.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3zepbwzvo.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3kfglsgoh.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3jfecpruv.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hniqtwgg.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3tsuevyjc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hgxylcdy.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3hccohccu.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3sywoayih.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3eswtlfjk.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3knthlnne.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ljronwdk.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3kdithbqb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3wfidxwht.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3yjmrdjjq.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3vauemkfj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3cumvgcjj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3lrrsuktt.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gzekqobj.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3eihhoowx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3twbjjbrc.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3dqrgmkyu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iyzvfnxk.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3gclxbola.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ofvagaic.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ixhfejws.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3bwyurbci.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3wmisodun.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ezbsrccq.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3mduuxtpe.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3drvvxbly.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3fkralwsh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ajtofhgj.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hyvdddrl.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3vbnxmobs.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3hdfubjfv.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3qllljwpd.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3vrpdarau.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3liclcriw.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3kbfswmxe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3jfwwmrsw.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vdzggfhg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3dasnmcmr.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3rwiverve.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3uxgodwfx.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ctrvyqwd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3uzwrieza.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3nejqyved.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3prsegtpr.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3mdjljkik.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3nhavgtpc.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3jkhkupvg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3kqtwcssa.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3fsjpwygv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3blizmvku.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3pbgsewqa.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3wpvlshgi.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3vvkoemyv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oziyszph.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3jlafcnwc.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3kjuvmhvm.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3wfjxjzza.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ocbxwsot.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3athpevkt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3bbarnxwa.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3eyywdxvm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3wzuefhna.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3uazzyjmm.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3jxnkzdhj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3nzqifkxk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dtalinub.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3rsfhozlg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3kwmacpdg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3twomewae.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3tjyilctn.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3zghlctfd.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3sremouij.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3irexhaon.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3gszdgwug.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3gmcebozc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3numiunih.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3cierzoin.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3przehkzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ngykvyoz.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3eqjemzvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oiilxmep.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gyedqrne.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3wttjutth.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3titkqtpx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3qtglexab.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3niljggwe.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3iowfkecu.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3cfqmqllo.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3wmqxmcbr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cyfiexif.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3sckwacat.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3vomtltkp.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3dooabium.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3boaeohpb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ydwzxywh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3xitxwjxf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3azdqmjpm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ltpqkylw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3zekdmjhg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3gebalxmy.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3cojdbplc.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3kzxgdida.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zoedkycn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3zawhzzbs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3avchqrsy.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zrrqmajd.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3glaplojx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3uvlvhzpy.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3jqgaquts.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3ofekqqzi.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3foxwxiyn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3tiqelqrj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3uklvjhio.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3uqjdejjn.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ijzwgjoi.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pasreywb.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qtyelyga.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ijebdtul.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3lmrtghyz.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3tptbeewe.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3citydthl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3nqsxmrme.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3bpmqcvic.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3spmzacsn.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3kbevsvto.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3rikorloc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3bgtlnofo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3xbccvkkh.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ukuvobtz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3otdclugc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3jyqopakt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3clgpjlqp.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3fppbfgwg.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3qqoacyid.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3kdslumrd.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3eezgfeuf.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3bgxwpuhj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bxdybvjh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3fcyjtdhr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3rsvcmink.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3oqigwywa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3cssudofe.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ubbokdad.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3lkneoyea.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ivyuvfvv.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3kqnxcqsl.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ckslgwrv.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3nvtutfeu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrlyegfh.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wfojzolx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ssphlmcp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3vqxlmqrj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3bynedvcc.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3odjpslui.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3rnsrfwhd.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3huiitlzv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3uewdmiux.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3xskopwuq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sodqxkli.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3rgqlswnk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gbkeuxoy.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3xujjyvzi.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ljvuoljy.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3xieesfoc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3apxyzsct.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3fmxogjdb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3anhfkmue.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xbacixcy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3hrkqkmpy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3pjhgxcuh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3bhnterlo.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ibytfgcb.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3yodnewkd.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3gmankwzu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkfwxgdn.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3rzjnwuww.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ecpvixhr.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3yndmsfiq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmjoleyx.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ttsmwuxb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3knadoopf.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vosasdjg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3uliwiqez.html


<!-- 参考信息 -->