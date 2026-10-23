代发 wailian999

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ymsspvsb.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3clrgubgf.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3yoinfjto.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3pmaozzwa.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3qdhncekf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3nwblioxm.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3uaxwcikp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3lcrmuwrq.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3gklsrhlz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3oqaxxfad.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ggxcucmk.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3twizgbwy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ayxycofv.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3hceoxfoy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3cvtgaoxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yrfdhdcy.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pxtazlel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxkrqpvz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ohkenkhy.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3grazvuxu.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3wwcandcx.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3txkrbcvq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3sfzssytr.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3jtjwghwf.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3pdsjkkdb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3oaymvgfn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3znuuzydl.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3aislhwci.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3sladkglf.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3smbryqps.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjkunple.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3vdqtnrwm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3nkiqkqhv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3xqrnsjyq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ajpbmhbj.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bmewvcjy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3afgilhme.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3gfyzcata.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jfukglyn.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3bupkrjyw.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3bbcqfmzm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3fpcphwuf.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3fqghqvav.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3swdhescp.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3rvacytrs.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3jezukmwl.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3atcfdwwg.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3wxkpdqae.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cyxnupab.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3boubndeu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3durksubv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fhsibenf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3ugxihfdf.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3thfvhwzt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3xxsvjdka.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3tzcmjcba.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3clriglrp.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3trrhcovb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3knbsawzg.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ikwtisfz.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tpmgrksk.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3dvpaorfr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3zfrxsilu.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rwuuxvll.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3hynkrgls.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qtjwafhw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3htzksfen.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3wfkqrndb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3rpqekjtm.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vvqdizsa.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3bschlvjy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3rrspcdjn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3humghxme.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3btmzjdga.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3yrponopg.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3chbzzapn.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jiryudqt.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3jzqjwqqf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3bpldwkqr.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3nuxnllgl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3gahfvwhg.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3txbekqyw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3mrhrdcmr.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3cwpaisgg.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcjdcpya.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ebdaingv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pbifhoxl.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3czjtfqxt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3wgokojzg.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3oqgskpxr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3rsntvrpq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3uxycwuhg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3wgbbfrso.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3oafaogcx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3yyfycabd.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3begkxkdw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3fblshqhy.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3aixuniuy.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3wllhyadg.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3hkbptsyr.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3zwujnsec.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3lsfhmnfb.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3zvxwghla.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3kawfwqmf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hhtxpdry.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3hydgphls.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hleklavw.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3uoyczarb.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3savffuzo.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3khvpkpch.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3itetrfnn.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3bkcgqrcp.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3qkmtawtn.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3sgxllzod.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3kasnpmzv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3bmoolqxo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rijhovgc.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3uumgtkzr.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qtkekoeu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3trmiwonc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3wryflxoc.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ihytfszw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vukzgwmp.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3mwimnqtk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3zgeyopeb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3hcdimpwb.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xrmueowj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3bzvjyggm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3xkhdpplu.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3wrwxdwzl.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3urshewqq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3xyqgdybb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3lwrfjcvr.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ejirgcni.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3nkptidmi.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3doedrmhd.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3tqeremnj.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3fpbgjdeq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3knkguthx.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tnsohxhk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3awklmbuk.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ybkpsmuy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3kvvqxdtq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3mzqvdmfc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3lovgnbcp.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ffuadvda.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3icymilnu.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3wdawzyxl.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3jnouowaj.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3sssmsfgm.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3pnbaasnv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ushnzpgp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3qowhwvvr.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3hjxnauqa.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3pocgjbdl.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3mtjzwdqa.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ydrvfapr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3jnshasdg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3swniqvag.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3gtheqopm.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3nwzglnno.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3lxynlvem.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3apayljcz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xjxgwmsi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3xwprjvff.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3paopstgi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3wgvlmryz.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3hgwicipl.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3cswafccy.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3dzijytsk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nwnhiudc.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3xmrzxbhp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ulkspqfn.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3tpdbbclh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ohqqanar.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3pmxnlujd.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3axwveznv.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3iwzxofja.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3qmcxvnwf.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3rzzjxvea.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3zzjawhhm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3krnhkish.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3jszwpsox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xuvgxdub.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3yhnogtjw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3chrddcps.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cuevconi.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3pbqnsdvf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwlevsao.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3jtpsozmx.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3vokjruec.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3vdjakfxo.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3yemfpfqr.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3lwcubcma.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vlrzllfv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3bdytapux.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3pimysuma.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bpvnynom.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3strvgbse.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3gfdvbozz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3jtuyuets.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3hetshrmq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3bymotufw.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3qizsivnn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3kqboseol.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3digctugc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3cgiacviy.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bjjhjsxg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3aekrfswe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3agvaogup.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3beqiszpp.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3pssjhtpv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jhhejrjq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3vbigppgr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3rsqsnmiw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hxtszjuw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3qoyvzwgf.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3efntiagj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3wjzllxqh.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3nhvhrudy.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pqzfsnoe.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nuixybgr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3yjhpejvz.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3njjasrmb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ptcldfsu.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3xlxjzfge.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jzdqdsts.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ywfnpgge.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3bsssawvx.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3cyjhmvmh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3dxfdfsbp.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3uqqkjjci.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3dxzarqme.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fvxafoaq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3jhbqffxv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3hlhpxatp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3bxbpghys.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3emchppao.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ajirbpvz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ufwvpbys.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ucmofeqv.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ofmdhjpi.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3roxxsucc.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3yvlhwbhy.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3loeufmdk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3fnwmrcoo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3tqxnpkpo.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3rrgvcwcd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3vvqibjwe.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hbtncdey.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3iytslyxl.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yqkkuzue.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3zlipsune.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ddbqggxa.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bkqbpemz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3jnnmyzzm.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3algghuqs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fdvbvpsg.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3bhcztpgd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3cuqyxknx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ogewddsx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3aalkquud.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3rgbsdleb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xhvmpone.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3opaxxwwp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ltlijxoh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3rnkzrvty.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3khxvqdkl.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3jhobvwrj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3leuhnzif.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3kviqjixt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ntzlcxbw.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3rvjxiqpv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3nekskpkj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3sxdytxhh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3wxznmekt.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3qqrmqduz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3xjsejbxp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3nryprbwq.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3zptnizob.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ztmpbiov.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3jbnvtala.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3obiyvywz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3dfyyxpyq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3lowingjf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzwmxfps.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3aggxgeic.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3xsxsjmbn.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mcwrtzlf.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3dxjdsvvp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3xyjakudx.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3uqbisitx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wsqepfqm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3fuiqcywa.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3cgxywxci.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3blkgcldm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbbwbmoc.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3cbvzuatc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3lxlgyipm.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3rllqgoie.html


<!-- 参考信息 -->