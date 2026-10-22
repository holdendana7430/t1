代发 wailian999

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2lwrbeclr.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2maicnvbu.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2bnqyxmhq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2spqvbhlh.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2kwgcjdfc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2nzaxiibh.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2djkzicse.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2hgyrscwd.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2zrfoyfmb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2jqzsfpdz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rdojevja.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ewuadtuq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2abvflrxc.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2bgbaxxbd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2auchtlgu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fnivdnbr.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2snolxjmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sdlsygky.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2tlhywvdb.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2vxriguki.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2bwvcqjbf.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2zmkqhwhy.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2luvuxyuo.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2qktyqbil.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2xevimxdi.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ihclpwoc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2mujmvvcs.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ekbknipe.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2orkvzghl.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2gipawptv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxirdxvf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2effcddwh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2gxlbbwjo.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2naathbhx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2fjjqomtc.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2oootbvtr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ayodkspp.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2zyaimwvu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2oemfigrf.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2uujqcrcp.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2rymwrhxg.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2izvawcch.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vmxddtpw.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2csrhdqbs.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2mzsfksic.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2sgkhrmut.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2fuuvpgya.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2kkggizkw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pzipzdwk.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2wuqnmpkp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ocfaqbvk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eblmiuqa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2gtffwccq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2zswtrcba.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2gxrxyuln.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2woxkftxl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2mtpnttet.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ehpakbxn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ktmhfoaq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2otdcrdtp.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2wmygkzfz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2qcqwqdkq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tqecuglk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2kqoxzfdc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2bkpriftv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2hsgzorsw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2jzxpiubg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2yywmaxoh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2gwgylzhh.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2kjkdoqha.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2qcgtekeh.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ekwvtwyq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2kaastrfh.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2rbawknqx.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2mnrrnqbr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ypvfwedr.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2paezeetk.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2uxuhvmfy.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2huxvzcmq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ctdfgaxz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2wqsfcubb.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2brmxbics.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ynpjkrne.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2xsfgqkkz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2jvvwlfsq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2vkdcrglm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2fsuvmzve.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2nfrbquvo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2bfcrsmva.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2cfuwubjr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2fnrlsrtl.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2nuhohggz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2nijphtph.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2klphtcoo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2twcckfoo.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ahcfonft.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ujyowrcn.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2tjktslvs.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2zqasyyit.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2dmuzwaae.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2edngqjsl.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2havqihtp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2bmrewlir.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2myhyepyt.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ybonewmp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2mpybhpgl.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2kanrjwwh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2yasfrkhe.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2hrgztkhw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2gogkunrr.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ulaxvdmh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2trcymucx.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ersoonsr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2mijelxrh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2jxbfpely.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2odwcqadl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vjeurfnr.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2msbouztt.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2shcfolmt.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2dfqqlrjw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2rbqcclqk.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2apkwtgad.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vkebohkd.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2tvpiksoc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ebjrtufx.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2qvmafxcm.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2aanqreiq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2pachazve.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ullrxocm.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2hhobvnon.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ajvgixqp.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2dibmnlnw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2bbamyvue.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zehkodmg.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2pcurrwoe.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2zicgucdz.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2fgqzcasw.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2fcjnovqz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2yqggkqgx.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2frwiziag.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2btgnwfnf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2nsqiaror.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ckpxzyse.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2zfidrabb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2mwjxjwse.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2naonbvsr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2elculqsr.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2nlzoeigp.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2czzbjlwg.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2wsmgdgjg.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2erirpfeo.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2xddvtwhd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2etozkjoz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2lskupzqr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2btrmuwqu.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2lzkfcjuk.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ixbgtlor.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2etiwcicq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2dfujgzev.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2lyzjhtma.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2yzcjcttq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2uvmmcqva.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2wjcnveck.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zacguomd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2nanxxpjq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2cigggruf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2rejvvsfs.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2kwxynowl.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2abakdwpd.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ujtrnrfb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dazqjwfy.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2msiurcfy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2shvljuav.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2exbegmho.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zeopwlll.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2jlarxyne.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2pxynfyqc.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2hcnfbomc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2bssouiop.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2cgekwrtu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2lyffousk.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2zkzosiqo.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2yocaeofn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gmtadrzk.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2gionxbgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ufghziaz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zfsvkokc.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2sdcdtewp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2semvtxnt.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2iozljezp.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2npxgwfua.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2qvcezenq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2utrbfgjm.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2phzeytzb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2shcsujnb.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2itrhnsvc.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tepkuonn.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2esvwwjfk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2idqyoixy.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2xtreeizn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2rmfjpfol.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2yedelfxy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2kwymvdny.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2oexagfcd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2rbvjjkel.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2hrjunoxe.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2hrmodtbj.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2unabftwo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2wvbbhlzm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2pmynkklf.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2cenlpsqm.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2wvihctxe.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zzapjoxk.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2rhrhutor.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2rcwluiex.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2jjdpalrt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2gqmgowsx.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2iyulhfjv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2hupsczwi.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2xkkxsqat.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wdoqybpk.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2alkzlkww.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2tkjnpfdk.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2lidmuivy.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2fjhbxlop.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2stgeedln.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tmemkisq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ctfobwjn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2flhugzco.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2cplkruou.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2qqtkjkra.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2dpjvgmel.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2jarzbrcf.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2eabjpwis.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2kvdqcdvb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2fezkvrtc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2isicxtfr.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2yqfpstnu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2gtualjor.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2zazxvpeb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2dimbaozk.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ypgadsbf.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2revajwbe.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2cgnwjvvv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ihftaotm.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ubuxbzdg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2fcmqzvhv.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2mooepurw.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2joxoocnx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2mkfwcvis.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2juaamheh.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2juhgxqnu.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2adhsmepc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqfwvknv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iracxzqm.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2mnvovtve.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2gvgmeger.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2kmtkgppa.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2gukgvzvp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ipctibxc.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2sirqbaqp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wmtdazit.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2wtkwmouh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mjyrsaoq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2gvlbrsyx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fkkxzqku.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2mpgbyuum.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ozsrnkkm.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2jvnvnsdl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2dohrqxqm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2fbixnlar.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2unspwfvb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mfiirlst.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2wkayduyi.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2wpdifnpc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2niuwjzhm.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2hlvdspws.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2khtpkytf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2cccswlnx.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2regvszwz.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2hxspqzoi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2nesnrdje.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2dyadjxcz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2agjdzsze.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xukswdne.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2yxmzgehb.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qlcbfdze.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2zaiuudtm.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2gssyywhe.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2akjwxhaq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gjorgtjd.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2oosowsjo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cisnjsby.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2vphedspj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2wibkkezi.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2rutmekej.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynkegluy.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2yscdcbrm.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ipweadoc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ccfffsdm.html


<!-- 参考信息 -->