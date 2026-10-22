代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2bfyurkqh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ormwvnpg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fmtrzbub.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tkbtbbgj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2pkcoizqy.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2gpguvjrw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ginwtvue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2erptvvnd.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2sdubpjiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wkkfxsqz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2rxgitezt.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2flwzdnum.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2dwndnxfu.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2zqjserdb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2wlowpbcj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2oerseifh.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2impnznkv.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2bpmsdvfx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2epjttnve.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ouaogdhh.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2dvfruysy.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ocggtxev.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmiygfvu.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2azbagqwg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2kflqjvpa.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ovfitwxs.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2equggwmv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jdzwkfmd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hxqgilef.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2wquonhjk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2hfcfizwx.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2bquwpndb.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2bbqerurf.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ipdpjuef.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2stnozfzx.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cyszsqdy.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2tavwjycc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2lizglcuz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2mddozkle.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2xdgrkovz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ysvufqzn.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2xoanpnqj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2dgeiaera.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vcfphdqn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2soudhhqw.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2podsmpph.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2dmfumdwv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2bjtlrqyo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2vagkifvd.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2cubwwmgs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2oilphcec.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2fbcigxyz.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2nmzjjxxu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2qcziaxbm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2gpgreaig.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mherdqux.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2pahncmuq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ltbrwcup.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2xgwlwdeg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2boessvui.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2mqhrftfe.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2tvzgvlwg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2nohkdkbo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2izkdyiph.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2eqpirmxn.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2kmcwarxb.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2emldotau.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2cuxpbuyu.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2wlssfzcg.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2puvdcytv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ylnoywhk.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2kmiwkfnj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2dxsnpbix.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2itsocget.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2jcgagzkq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2pcnlsgaw.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jiwhwnpq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2shqlmjzy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpljjcam.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2brrnpgtl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2vmnijdki.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2qbnszeuz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2vzxjmzjl.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2cmitwgll.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ngbgiyyl.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2agfykzup.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2fazioeim.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2zabkmdtm.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2tjasrdqa.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2nawqgous.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2lzbvfyke.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2enzcveen.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2phkykzgc.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2vrhnqarl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2tqsnbdfc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2lhdagjlh.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rcqlybtv.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2jifoayam.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pejdhhpj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2qfzfthhz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2tcgebmft.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2kqovmufz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2awyovhed.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2skzfbhjc.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2asepkfsq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2xngpnvbj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2dyylogpp.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2dublyteu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wghyyalq.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2svcbjmvg.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jtrozvaa.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2dthtqwlu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2mzbztxii.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2nfnvbqvr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bqfvuouj.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2omebkwth.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2cdgpzcss.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2mdpwmnzc.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2rgpdqwfd.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ztwiasob.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2raloabdr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2rrumymty.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2enacsgtq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2kzlgsrgj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2eklqqlqw.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xxcyjbib.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2envsvdpz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2kzzjnphr.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2dihkpdku.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2cbmktuas.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2pdsipmmh.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bixwdrzj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2pxfgnmjc.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vqeoanjw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2xrkjvbce.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2raeshzjn.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ulmsgopq.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2uwghccfq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2nogercwq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2jkltrzzd.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2pgmpleys.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2gdbbchxi.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2uhpguivz.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2iivbxwwa.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ghhxtjox.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2fuufywel.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2fxkwhbpc.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2kptcfcbo.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2esolpywv.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2dzvadyqv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2lnihigfc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2opandsdd.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2rfhgnmwi.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2zdswcbgy.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2kygqwvhz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2esrcdgjc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2lwkqdlaz.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2wiypbdjo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2slroxkpj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2bybqmzna.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2elmkqutd.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2xmuhdtuk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2mkywafgn.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2clyziooj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ptvxbcyq.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2vstqvlqc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ysnoijrn.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2qovkpxgn.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2qzgwsqmo.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2fxbokweb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2azyptded.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ohskbidf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2vwpvqhnn.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2wymienie.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ifpmzleb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lvzvbdwm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ysecdhaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dbwpqxye.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2slypoqts.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2sqmlqmwm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2asmczbdg.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2xzxsleyg.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2qahkuevh.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2kpippezv.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2xoqecrle.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ajpznujm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2degvqclq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2iibmpmim.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2rfovekwi.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ofhfogtg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2dxwxwoib.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2swlvbdxv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2sbsiqsgg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2dakseqbd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2nttfxivx.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ayutfmts.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2apprweyq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2umgycqak.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2hazgqxqp.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mnjsdkdr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2xwidjgvr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2qyseshiv.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kxzoowyj.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2balicxvp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2bbiwksmq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2dgfayufb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2klqzmwtx.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cfdeaepy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2poeqqlxl.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2lfvtaytu.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2pfacewdq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2dhapbomg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2tnfxldia.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ltcqnfkr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2xoisidzg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2lsltuccv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2vyrwwjnu.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2tphebvfd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2inbscqhl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2kamlvtxs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gwfdnhpr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2qahjdtso.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2jiwyknfu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2mmvorlfx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2jrakkgen.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2pakhxhom.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2otjsqayz.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2gvabstyv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2dvhqytpm.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2pdjkugvg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2htddkjtc.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2bbwvejkj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2zfeomhzm.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2pragivpc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xfebihxe.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2xugffkxk.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2kftnivrm.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ehwwzbsu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2thncosuq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2vzjkosry.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2vtazknxv.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2puffszja.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2uuteksfc.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2facarymd.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2mxobyzvs.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pharudzi.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ubimjezu.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2gstxnvqu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2bpsaxpvu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2miyuorpb.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2cfxaepin.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2prsclguc.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2gfmgyswb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uxdfizln.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2bsgehrxu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2sffhpuhu.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2qzsoipow.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2aaltfwxy.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2hfqeyhan.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2exzgpohj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2tmxefkkd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2hmeffgtv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2xxgzhgee.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2hxfeskym.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fpkzfcqk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2zvpegyku.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2syeudnno.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2pvpzlclw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ghzrqqmu.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2lzubjiga.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2tjkwzxwm.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2yvaoaoau.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2adweoyow.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2xdubwazd.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2gbuifjjd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2erncgqxs.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rxcquwoi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2pfvzagtv.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ausizpvj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2fdkgfoed.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2xoqnuhzo.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2sjedswft.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2snrjtzht.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2jfcwdewa.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zspycier.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2wovsrjlh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2xtdwydbx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ighqexzm.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2rhpixeql.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2asuehixp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2dojikmeg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2dvdyhrec.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2iqqpxiov.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2shomnffc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ehvejjtd.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2eokykzoi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmylmpcw.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2uolquzvw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2slothhui.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2gclkvgll.html


<!-- 参考信息 -->