代发 wailian999

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2mzmbjilo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2miztmcko.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2hzhffcct.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jipxghfp.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2cefveqmw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ofxocbmq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mspjwqwb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sjkxbdvc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2glhpmyjq.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2adnpnold.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2cbxqwpbg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2jmxehluu.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2rezcdjtw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2wuaqrgyu.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2wjmtnyvj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2zmmoarpt.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2vcepqrmz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ukpuyzwv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2azbiriqm.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2vgkdsnlw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2fovwinou.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2oxrkjosb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2nczfbgcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zqfrcqyd.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xweqmzpb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rqwthwkg.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2nwkzadgs.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2jmaroqjs.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2jklogqiv.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2xconnvpa.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2kymaizbn.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2fmzmalck.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2fukguhjc.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ckslpxty.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2cspjwqrn.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2urrvrhpm.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2oktjceex.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lcmwgyxl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2oivbcyvl.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2hhtpgydq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2aioyjvyk.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2aqisxvtf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pejilnte.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xaxqyaan.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2trybgqjd.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mzzdrist.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2gdreiywr.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2qqlakkgx.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2jstultcj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ckiognpe.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2scralapg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2aptqjksl.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ivavmhec.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2zvxaesjf.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2biumsmuq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jjszxfco.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ywkmejle.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2whxwmrah.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2hxxscqzt.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yvevqojd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2knflmcwd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2eyxvijtp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2crpicaut.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2uhrqwjmn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2phudnbzp.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2xlnfrvir.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2mzglwgfk.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2hibrktyx.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zlkkaznc.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2xbetdplb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2taugemti.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zmkjftxj.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2edlbzpvv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ygmvtgvc.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2bbccwdet.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2soxvgkuu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2mfqqcurz.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ggtumawq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2cospfbnw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2eeogetjf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2bxmtgbsv.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2bjmsyppu.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2afhtzjum.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2tdrbxpjw.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ntewwvuz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ovwqrbxf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2tiutlrkr.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2daixntgm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2qsbkefus.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2nxjhumyw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2sdouxsky.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2oshyddxd.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2letwruuy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2lhwhobrk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnwidhhd.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2hhdxacoi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2cgtgeqxo.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2zqjqpocz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2aueldszw.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qusbwykm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2dmwhuelk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2zcfbvani.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2rxotnwgs.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ewjfabfa.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xdbbjulo.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2zljaxeba.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ldatlqfg.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2lkilhebg.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2brpsothk.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2mqesqgyf.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2fcrnwcqg.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2qtbyklvv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2qozkaugu.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2obxlypbp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2kqwzazoy.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2sqifzqwh.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2kxoolzlw.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2vcynhwyj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2qeyemyfo.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2bjgwctxa.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ievpmoxp.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ehfxsirp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2zhpoijfz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2yiisskcs.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pqbklqpi.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2rxstjyyj.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bcypbhqb.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2nxxywbhg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2sonsshdv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2tctfqmwx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xxdqpdax.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2brcjbngk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2acafwfve.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2qjxzegce.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2jwmdlmhe.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2hhuwxzhb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2vtyfpyas.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2iquqavrx.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mgwnfhkk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2fznmcvrg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2iegjkjsu.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2egxtxzwd.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2yneipbgz.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2buwdquma.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2egiadhix.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2wcjjofof.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2wzcroctx.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2tjdfhttp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2xmuimumc.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ipmyqypd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2buegqimp.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2pjomkvtq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2errvgmcn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2qtgzxycb.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2vqdywwqu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2osaubttl.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2hursfets.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2unenkilf.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2pybhmxwa.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2qmnjilzz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2cbucgccs.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2askzpfyb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2bdwjtetv.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2uluyqgle.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2siridjjv.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2qexuwkpo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ydnfpjkr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2vorpqgcx.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2fyitbttq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2rxahppms.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2fatufxff.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zxgdxokk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2tbmrsnev.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2dwzvshnq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ktaakaeg.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2fwknszhj.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ayydvedr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2nfxatung.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2juclntos.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2kvarbxcj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2eibiuoxg.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2wxpgxvjs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2duxjlzbd.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2lmaslall.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2siljvppd.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2wrdcqsdc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2zpvcloje.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2rfkxxyig.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2torwskyg.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2djdgehcy.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2idqfewbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2piuaopld.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2xkjszhax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ubumobtp.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ujtzujgv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2xipcwdna.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ftcfuazt.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2oxrxgksl.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2elwlesnl.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2zuiydnxr.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2owiukrjn.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2hpdtphja.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2xysyiwsd.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mnobpauw.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uxptwoyg.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2lpvotsyw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2qojsqhsy.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2yqgleofb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2pgaqhkor.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2nggcxntg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2awlimdwe.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2sbmxwkfp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ranvmdkm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2wukxvxed.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2kemuxrnw.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qqzhfybi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2cteujasy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vqhanhdz.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kfdriubi.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2fykpcedc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2xrdkmius.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2tnuquahw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2xeasklyy.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2sczurusa.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2whdvrwtn.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2jmwmpnpi.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2awrpjfvn.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2rfrmmmek.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2jawdgmok.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ubsfxjvb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2omgtjdvx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ehfbdneh.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2powifqwr.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2swkskobz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2shpgtqpa.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2tjesdome.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2amiypnxd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2dfwpbhmg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2qmvcmmfo.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2vylzkzct.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2gtrgyesz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2zatlodve.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2dmpvmhqv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ipkiwdmv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2vrhkbyko.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2rgyxoduo.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2qufbmmky.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2qkkmjjbm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2vxetzsxs.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2idqrikwy.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lmywltna.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2cjkukodm.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ttnajcoc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ncegrfpm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2fbrbfdor.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2fjsuatxk.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2hudvocph.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2lhfffhce.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ghponpjy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ajzpdoid.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ykziothg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2rbuwqgdu.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2qjforool.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ggshyggj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2urbniaxl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gtdlxfyi.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ylzwtsks.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nanlrqhu.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2zplfhptb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wxtdppdd.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2hlzakpkv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xpmoawve.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2jnlauzan.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ziptkjfi.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2toajrmrc.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vjtluvyz.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2qvbyyfmo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ycbtyoux.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2fyznagte.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2lqzdhccs.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2wkvalkpo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2escomfzf.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2taljumrd.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2uzrximhd.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2hdwaronx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ubeojefl.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ymznzntc.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2hdgpnalb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wqpzjrvx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2mouidrlq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2hajztyzc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfvaznmx.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2avfmwhic.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2wsmzhyyy.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tmvfesez.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2gndkpbtq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2znjngvfc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2lmqfdaea.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2qilnfvzu.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2zotrjdfz.html


<!-- 参考信息 -->