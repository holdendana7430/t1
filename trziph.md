代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3blnqpwex.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wmgybdsc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lhscwdnz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yzuernoi.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3bfhlvpph.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ssetttey.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3tracstla.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3mvkbrpor.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3zzjsagxs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3tbcnoccm.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3uglxkhub.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3kddqvfvk.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3mpidtphj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3kwtivwgc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ylgeunqg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gpghzgem.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ypivjdsz.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3jwfywgqn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3julsibsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nhwlzgfd.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3dbxdywln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xqpjcynf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3pvfxavzb.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3gqiyucdf.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3jjuijvfe.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3wstdckkd.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3bemknqiw.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3wenrxtsr.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ifkdyzub.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3tadlayou.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3qxtmdoey.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jsqthabg.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3pbmxpahh.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3chpebckt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcngncoh.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ryfvdkkc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3snuyulll.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ufporsxw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pcwebbck.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vxmhycjn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3hpjxbblm.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3gshahdmp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3aciypban.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3gomgqegg.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3vcgekssb.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3xzlthegt.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3oxpbnqll.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wgczotew.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3nwrrcgwu.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3cmloeprk.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wmkrkkxj.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3cyxyhjxd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3cynuzuzf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3pesnwzim.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3nuvtzhan.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mikssjqw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3wbllenzv.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3klevysla.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ukaehjyo.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3plmxgcbu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3wtdgvkum.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3idzbwkqz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3bqallzks.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3wvkqcyta.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3trkgwdkr.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3alwlnosr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3iwextmub.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lwqyodwm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3fbrypejb.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3sieqaopi.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3foybhgks.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xlrcezcs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ijetuiwj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3biebpusi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3rmvaajbw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3mibsltbc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3oskdpgtl.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3vojmobgu.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3zhflutjn.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3zzfkzdtm.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fpsnoovr.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3aecmxsnl.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3forrdbey.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ivizkymd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3rkerrltd.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3grjnnyvz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ijrjwpih.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3dkvovicy.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ppgmkydr.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3zvvehzor.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dorlinrb.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3rbzvlmju.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3xniblxbb.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3lzirpkxg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zfijllrc.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3bdnftdhy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3akdknrcs.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3kdffepps.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3epigsdxo.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3dgcpmtgp.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ghzyiszp.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3gevftftz.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3xgqoiqya.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3iktpqklt.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3tlncjddd.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3osiidomu.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3uvnaexaz.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3fvxmmqdg.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3nkhauvdk.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3jildeqrp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mkavdbek.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3bzwgsvqn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3taobnysr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3lbajrnwx.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3osuabpxp.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3yugrbfpd.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3osjmvhhh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3rkwfillp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3gpqbxgsv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3wkiwrodm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mlsgosil.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3hkgtokqh.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zqwkrodc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3cyhwogab.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3aslhuyde.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3rtzknzbc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jvbizoty.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3zupoccrw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3uevddigm.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3pedmgfvh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3cxnlziqd.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ibeyctia.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3rbjtxpqg.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3gqqwaupt.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3abdyiwaz.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ulyucvdp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3zftypubz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hjwhrhta.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3undowhzg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3mnosylef.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3puncsate.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3qwsjhisp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3vsjsgnmc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3chksossd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3oiebrcgo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ivlaexzu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3iznxtcgb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3leufhnce.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3iqexjhoz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3faxlumbx.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3sxnqldyc.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3orbyfrfm.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3reiudqam.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3urxpykao.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3upbbcjks.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3feshyxbb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3pqfcwvtq.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3gxscwgqp.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3bbcvgdtr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3eabetnhp.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3resvroyu.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3btxpprpa.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3cnvximkg.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3swsacdwb.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3qzvkbvgc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3jfbgsnac.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3nribkzwc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yiobldbq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3bbgworyw.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3yyexobly.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pomuwvyh.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ifcjwljv.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3jsxvafzi.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3gaedtxux.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zkzcbdlm.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xmcqabbw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3swzzpdwr.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3bvtkrhie.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ffexcnkt.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3uhxzyubi.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3zwgcwngh.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3nlalnyit.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3nfrzrfwa.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3whzfuzzv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3qfjrymoi.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3tttstaqt.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3cttuojoo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oqzmvdlq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3iqgaywxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kldrnjvh.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lcuderdx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3jtkbbqkf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3dbfqcfvw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3trlnexcg.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3wigjgmok.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3oguavwjh.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ghlstgbk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3cfmagjgv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ftepmrni.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mwjfudet.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xsojfhdh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3luutfrvv.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ixhakurz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3dhnopplq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ccuaffjy.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3tmolcqhh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3tbzqjmuj.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3rhzqghij.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3edhtsbxg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3nbqzsemc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jsqaikfp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mrdihwzb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3woxbmuiz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vndepziy.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ccialeim.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3aoeaklgo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xgdxpcvr.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ybetnjyr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3jyzjawjd.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ykgmvgjh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3myzeuaob.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3nmhmhtvm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3sleuxhae.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3yytygggq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3vpvjmwoo.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3opjuiyrv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3osuztqrv.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3muotsreg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3stmibrls.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3rrgdbsrr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wvrgstfu.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3vqyseoxt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jdpxgjcb.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3zklngmgn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3xjobwdzy.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3xhnfhmyb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3twkixpbb.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3rkazajtw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3wbxjotan.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3gzsonheu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3swoaradn.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3eouyvnmw.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3fbbmzcsp.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3nhmvlpdm.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3hsovskgx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3qukdtrgj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jickocpw.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3wdbqpfrb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3lbvrjtwf.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3vicfblws.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3azgpeihs.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3dscjckyb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3gqojgbgz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dpfnzcsm.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3phtoukzl.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3klhwnkht.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3wavknrww.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3xygtrvpe.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3kmpnoqaj.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3cqyvqcjd.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3hrnhahdz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3iuyoliqf.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3bvcrnxkw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qujmdiox.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3hdusgysa.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lttbvois.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3vpttzxkf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cxhdyfsu.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3kmidfsec.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3pkfvnfpr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3hedkipio.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3heyvhkei.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3uxftfpfw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ipauruod.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3uziqueqf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3emcewqxr.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ggyppsbo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3vgsuqrnz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3lmhitkic.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3qchospwe.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3uhahuvtm.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3jqsvlyuo.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3mwhnhtvp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3qweuyytd.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3weyfmywt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3bhxtvdzx.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3hvoynbnl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3drgwiwpa.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3reozhwyi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3gcplroja.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qlobssuj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3lmbmysew.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dzqavfob.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3msnjbusd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3hbonigbn.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3wmoecpad.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gdtnvhsi.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3atmqbuvd.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3rjizccfj.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3mhracoby.html


<!-- 参考信息 -->