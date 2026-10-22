代发 wailian999

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2rjydgiar.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dayomzcd.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ozrqdtke.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qeccdztg.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2uzeeygtp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pyzjxsnj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wnbjekph.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lsdcmtgf.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ybclmvyq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hasqxlij.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2iqeyonxq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2tfcewmne.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ydmycoik.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2sfnhukdl.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ofejrncl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2kbmuvhxk.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2oswldfbu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2upijqsnc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sdlraqmp.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nowsvjzp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2zkhtppas.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2xrmzefec.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2jwhxzlkg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dsxeuyxc.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dfebuvrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pfkfcsbl.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2glzbrovc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2npfmxjdp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2rwlmzvxk.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2htkfqyix.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2pahaaqtl.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2hwbowmql.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ntayagsb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2aacaxxqo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2dhnhmaty.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bgltpncz.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2sankostx.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jfzxeijx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2gktsefmk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2svxkncgz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ehmapjrv.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2wtfoeyud.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ovbrnmpu.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fpxlrugm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ejdalbar.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2dhndazsx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2xvbxxgpk.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2czzeignp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2wvligeke.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2tfiazuyo.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tfekxohr.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2aevvkpdg.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ozdlnygj.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2bqncsgke.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ozaiwnwf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ivmvyorz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zapqomrz.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2fmgftgym.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ofmccxup.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wuawvuqy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2efkfbbld.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2hewrcbeb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2lsqoscvx.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2mnljgymm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2unuwygaw.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2tsizvhri.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2gjplpidi.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2rsrndlvw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2gyudocso.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2eetwqrby.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2zvhvfolv.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lqydtdvr.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2zkoqjxxy.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2drzvaqjw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2zibfrrjp.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2kqrxhtwe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2wmoaemaf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pwowbmel.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2clezjgvw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2nptowxrw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2hkpekzuj.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2auhgjdsx.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2azelqcws.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2upsynzob.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2mxrfcvoo.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2hcqdwvud.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2kxtkgpsa.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2pzjbxuej.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2baumlabo.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2vdkifwdl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ogbdcaqc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2xorukikz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2zyqauukv.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2vasmteng.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hozixaxp.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2jjdmaoci.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2kpgcnncr.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2zuugjaty.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2dpkocbin.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2kzinqquf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2hpjsreve.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ahykydib.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2vjhbisgq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2zewwqhsi.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jcsxfhkt.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2csywajns.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2yvofirct.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2awozrwud.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hxnsjodj.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2khsmkfxr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2mfrgvank.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2pydfanmu.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vhmuhqze.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2czqsizdv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2menidyex.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2arlbuqtb.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2fotqbjzw.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2wjivgzqe.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2szjcnwze.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2famzriqz.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2oanbkrhn.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2tnxkgdgk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2mzxzydjp.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2unrtkbqs.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ymmplgce.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2nkieexko.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rezsvhvo.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2bdmkuwyt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ubvitbls.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2mrqalqkg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sdfwiddp.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2fckzyrkb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2maqylxon.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2moyhtebm.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xfahuhjn.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2wuotawkj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2gqksgtiy.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qxufomps.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fvpoeyzx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2icyrbsvr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2rwbbeisu.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2erlofkqh.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2tcpndsmp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2bksasfsh.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2qsqomlid.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2bdmdrqqx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2mvlgejxc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bwumdrgp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2frcgochm.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ugtgurwm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2fefbyjfl.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ehnhhwqe.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2nvksrmvx.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2oautiixq.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2dkbsthwy.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2tghzrlya.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2gegsabbb.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2exmtpgaq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2oqappkmx.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2uiilmyin.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2jgegupdy.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2boubpaxw.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2hqbawjqe.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2oneojwkb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2cfxapjrk.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2fgedcaxe.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2cadoqblw.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2sbistljy.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2sgahfsov.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2tqhwaudv.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2iqrvtjzb.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2yinftcfy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2cjjusjbt.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2zyfhakzo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2lpakllyp.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2wtlngaem.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2lyzxagdq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2baskuqdh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uahdvphe.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bkpuaskj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ywdmxaiy.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2atnlvylu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zkpfpdad.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2jntkcdie.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2npwsslxg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2exaogbiw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ozzvwxed.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2rukwpxqx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2qqmfzyvf.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2tnmxkfzt.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2jbuelvey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rfiutone.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2djlrhkdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ccjlrybz.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gwvjolcb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2flaptujh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ysatjifq.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2rcmeiany.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2tnmjieod.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2nbalsduy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ecdgtyrc.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ewvzrfub.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2cliieust.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wmcugbiq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ngnxvqot.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bbkdoxmj.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ihygggcv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2dydrijzb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2csotymuv.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ikughkgg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2itozrdrd.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2wowrgphy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2wbcssqhg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2obibnwcq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ypsktryw.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zeomeqvd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2twlcsuhy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2lcgiccah.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2bcnncynd.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2hzraqpba.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2leswvsrx.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2orgspbcv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ymcbhisv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2bqixlcgk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2urqhthht.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vsforbwo.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ecbcmere.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2zqnlrsmo.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rmxonwhu.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qoejqvjh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2epdwylqw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2psgqtuzk.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2jnywbxxo.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2xmiviatj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fmtqlthh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2lcjgzacp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2soaxyafr.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2xtduhoiz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2kwzpohzx.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2vaionhcq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2umfydjtw.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2msuyqozb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2lilknnwo.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2uuavsway.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2jnwilica.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2bgdbjdvt.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2xqhrskvb.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2spwmpgav.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ogxymcbv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2yzlkfhgv.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qdsneiri.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2sxmuqmfe.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2mzgvsdkf.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2bwbzgehs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2xinbypbd.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2pzstetbj.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2nlpxydoe.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2yruoaepe.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2wvjwjqhc.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wyqniokv.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2xfigtlop.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2igqoqekg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2wbirywrr.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2cgcwuiex.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ffgyllvk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qcajdjjk.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2dctqgnyc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhvbzrup.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ktjrbmni.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rtbvfjfj.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2uejbmqkm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2avktecwd.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2zkyoquyj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2wdshwwpo.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2idycgrdd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zytvgown.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2xqthrwog.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2zbcfuasu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2ixyctqgx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rojczmzz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qcmzoxed.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2qkaxmlgu.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2cwtrxygr.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2mpkjqcmm.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2pavzfwan.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2etntyvuo.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2wspyoxzn.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2fmqhfpho.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2otlijdjn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2yuyfxbqo.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2sdddthqm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2igeieyzn.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qefoerqd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozozycuh.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hxnyyhxk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2kiekoube.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lvieqwqy.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2rzucetnr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2vecwmclk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2egjujffl.html


<!-- 参考信息 -->