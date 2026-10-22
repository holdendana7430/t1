代发 wailian999

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ytssyqpc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oilmcyro.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2icwfkfsq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dprgixwd.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2xuribssj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wugyaixd.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wojuipzr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ulyhllyv.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2fimsparr.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2brpfehec.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2donuzhus.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2yeuodhwa.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2sghsckcv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2pbivxofi.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2bzjzpnrk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2uyxxgzen.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2cnphwpww.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2rqqvooer.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bksflpzb.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rswlxtye.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2nzivvifw.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2hqlwyacs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2xxxmynyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kkeooohp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jntniwrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2adfwxyod.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2pjygphuo.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2oirfddxe.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2lsfrdlrl.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2dwtsmpar.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2fgovfvph.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2kjxpxpep.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2zazipstp.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ehhpdjrc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2fgujxbcg.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wgamijfv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ysdczfsr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2fajaxaav.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vljbxkal.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2hjmsheqb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2oumkygfz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2fygplywh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2gpxeirhr.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xyzkuxfu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2qfsstsrr.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jtbiqpoe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2nxgnzhyw.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2yfmbgonb.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2mwhepmud.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2gxhbmgyq.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2dbtnvqzz.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hiyhffbg.html

esac
来源：http://www.52xcode.cn/Article/details/gt2lhoufnpu.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2omlocwca.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2bixtatvc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2trkxrjlj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2syqvboif.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2oxzvgfbt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2reuiqhnp.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tylbdkhk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2xebyxqgd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2stwaotpn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2puyxwhxj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2fgshdtoc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2wyrguajv.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2kloqtxkt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2kfkhjezk.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2twgrmbla.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gatkuldh.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2huzmofrm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2habwjuwq.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cpjyvzwq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ukgubnua.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2pdugdwap.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2pifdjvdl.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2rzojzgut.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2qoeexzmj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2oogqpsiz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2vtomenag.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2hkkalmjg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2uwmnxmjp.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2drchizfi.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2fvbyzlxa.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2cvqkobzm.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ylxabobc.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2oneoyffj.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ayqdrfru.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vfekkwtt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2suqbymss.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2goclrmhd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2nvjjcvrt.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2pbbgzhdn.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2sfxnpofu.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2dmiiennj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ebsevqey.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2qrlwsree.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2nsdizska.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2updfqvhs.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2nralccff.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2qlqdbwss.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2wqyduden.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2rngcbyha.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ucnndtmz.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2qwsvvjji.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2vebdfgme.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2fnhnjejb.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2netolptm.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2tboelahb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2dgaiecvf.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2vhaocqhd.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2cvtaeylg.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2cpipwwbh.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ijrsheok.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2jbyncvua.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2qeirjomh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2gfiwogvh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fsmhkclm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2qvdxjaji.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2gizocpwj.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2hgjunsqc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2wzavnhmj.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2jstlvemb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2mftatrdu.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2rlgtbhig.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2phtrbkvg.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2fkkqwwby.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lqbyfijk.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2wqwxmbtx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2gueznzlu.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2wjzqyuir.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kvassmhm.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2rgmkzmef.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2zmchzlgi.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2zlzpjypp.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2khxolgez.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2wdeebjxy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ldkmejmu.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2saxifnku.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kpjmdjrc.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2gvzaygzj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2jhkqrzvz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pbiboorl.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2kktqrdhy.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2vpmqdliu.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2qplbnblc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2klghxxbz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2vwetsrro.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dcrathuz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2kthiwckq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wzsczcpm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2jawmncfl.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2wxzvrmdq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2wlusvbnu.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2zzkbloeu.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2cdskstmr.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2jbzahobc.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2pusdshcj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2nnpbrztq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2upgcsjyq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2kjswuixu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2zypbroep.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ezygqcwd.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2rlggoevt.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2hczzaqto.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2tlrlmetw.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2pduwisjc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oujegmgd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2qoqyktmy.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ixrxnodo.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2glfmqonb.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2jgcaykci.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dklwgdiz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2itllbpvn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2voitowvv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rblyyelj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2igserqod.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ncryabha.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2lkmrzvis.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bttxvnic.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2papfmbvc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2xwcgbloe.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2llkenpmn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2wndaewwb.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2iiokikok.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2hmnbpnaf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2yxfldvzn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ijdvzolc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2iplrofvl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2pikaawej.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2zhhbermh.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2kowonouh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vgigoaky.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2gerireuw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2grtwwrmm.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uhnpvozs.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2estybpzg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2pljmtiwd.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ktosqeof.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2fqppissd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2nehweiai.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2gmzfzapd.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2sttuequy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2erunmecu.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bfpgryxt.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2dikicbfg.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gqzrogdg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2erikqytd.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2lkigjbfs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2nabydqbk.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2dnpwevbh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2hronyrip.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2vzzrimgu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2nroaqoch.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2guuldcxv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2wlfxepjw.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yewygxgh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ngdymajb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ntnhzwbc.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2rjneoxxx.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2alsaojjl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2toztuomw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2gskkpkgn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2tvofepfz.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2geifxzke.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2wtsavbqk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2pakkljxi.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2wxwaxtii.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2kiapjghh.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zifkpkee.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2awefwfsy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ujwiffaw.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zdpvpiyp.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2jqasnyoi.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2tjfswjtm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nlcgzxor.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2xyhmwhgu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2advxazcg.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ndsnrzqs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ntmbdfqx.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2izrwkybp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ahloosdt.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2eolcnijr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2flqrwuhq.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2zesekpdr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2krvwepes.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2pqhmzxbs.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ybcuzjad.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2mmcmpdto.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2lfwaznym.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2poakujxg.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vgthyxjs.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2epgfewni.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2avptrolk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2aoabvkmz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2tigwlodh.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2osivvsfd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2nhzxaple.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2lvmwgvbp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2havfkaxk.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fbmbrffu.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2mjytnybb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2brdegbsx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2rxjxpznu.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2zkjpbkcg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2mtqiowbo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2etuatjon.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ohdnhpes.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nymtznce.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ktrecaxd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vjatmcad.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2vgwufoqv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2srmyxzno.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2vdfapwty.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2cxpboujx.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2mgghishm.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2scryaljz.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2bsnfbqws.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2azaphcgf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ilqqhhsa.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zeflctcd.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xauenbmd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2hcwuqcnl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2lazvpmlz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2mrexskgk.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2yerbvnef.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2sntzzidd.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2zeaoyxip.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2kxcfykpg.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2djpojpjp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2lglwrplu.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2cacfndyd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2fobsnjql.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jlnadwjr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2wuyhbpxr.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2caxbjxfj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2kzazrsaj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ivkjerwj.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2gvvogjtv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2sinfzill.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2stdmovoy.html


<!-- 参考信息 -->