代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3uvzygcbm.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3dfsqqpnl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3mitfppaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wskhgpkw.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3lthrzcwg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3baylqtnz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3xcihrqkw.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3dylrpljr.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3upjvoymf.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3kdywchtl.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3smrdhyex.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3gctsztpr.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3vgyvraxa.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3xxrugibj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3emnhzkca.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wbjjdtvz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3vwckledf.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gfuwnuud.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3svfynfql.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3mzxmmvsv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3exbssffu.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3mvlrjdsf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3vwxtwbkd.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3dveirzsn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hqeaseoj.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3nyrxmsgi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3sjjczzvi.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3qwtjsehw.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3twagolsq.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3kifbiabz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3qtughgaz.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ufuvmeab.html

esac
来源：http://www.52xcode.cn/Article/details/gt3kcckvrcl.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3pmctttul.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rfkxtynw.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3klgppieq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3rykbjkwi.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3itflaxsw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xwgsghjm.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3psjkofeo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vrseysha.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3xteghngm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ahuumeqf.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3rohrhgil.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3eehdigld.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ntrcivev.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rgdgvyig.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3vqmgicla.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lumjppiy.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3opeydbht.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3endddrce.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ewpylyua.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3leojewxv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ybjieaxb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3uebnohgg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3vgcywrgg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3arykzeft.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3htwzmrnl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3myajnfsf.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3hrrxvois.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3rbiwbsni.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3bqrguxam.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3bekeislm.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3vtaqnjge.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3imvttzkn.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3fumveuor.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3zdnbnqbb.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ajckijoq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3geuwxzll.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3isumjrlp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3rsfezksn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3klfaqksc.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhzjzalo.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3lrulcfmt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdxswmpq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3dtjxxdwh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3eoxqtsvq.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3cuenetwa.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jlajrckc.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3uvngzhoc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3cqyckcyu.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ulwnuosg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3lvfmftsb.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3zpoubbut.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ixpelnnt.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3nkzjcxuh.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3wvwhvxqo.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3sqsadlfs.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3urfdypwi.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3pxfryznc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3rfrzztoj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3cqcdlxow.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3lqtgorvy.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ysjrdrle.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3prxotfbf.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3cfltrkdf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3dtilzytq.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3tozvwaee.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3hkeswwym.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3dlkkwsxo.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3fesjwkri.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3kfldshhw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3yxiudkcx.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3rluhtjny.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qqambknk.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3fpaxrzxp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vpmrzcuh.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3xjuycmlq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3jwgzvhfm.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3tdmcaolb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zkfkviio.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3oevcmjbi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3sluxiaih.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3quabdfcy.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3umluewlw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3xfybcsnr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3yfdmgrlv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3hggbcfpf.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3qkmcsvuu.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3lfivacwe.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3yvttiuzk.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cbpxmfvt.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3bdujjcrq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3dddboror.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3nfjdgcrj.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3lelkylpk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3wqpyybxr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wypmacls.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3lvoucxjp.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ztiyukyk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3pvogrhtz.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3eyvpkoup.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3hjwhgjoo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3zdmjibtc.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3suwziklp.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3vdyitnrl.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3kuknwlfw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3nsjkxgti.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3vdzhnctz.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3bdhvgjwj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3qfhpwcad.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3wxllaabf.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3udshvtjm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3serkjksv.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3yojvjnpw.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3lbvsgmhl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3tmrdxgot.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3nqsfceqy.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3jfaclpvx.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3anwurhry.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3nyaesyeh.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gomtvddw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3zpqpdsen.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3hwhtdmbj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3bsdibkms.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ohmkibtu.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3saklxwql.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3rhyqedev.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3xfhnabas.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ljcwesmj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3zvrqqwew.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ofuowuwj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3azyhvmeg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ctevybsc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3uaemjgqq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3feflhvtq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3awzfgamn.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ehvgnnlm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3wabcitou.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3curbicwr.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3klwyeofh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fzzghthk.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3vfvzofsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ssknxfyp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pceyoskl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3gdviadwr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3bfvnxkrw.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3rfalatyo.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3zxhejohz.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3fstzwcba.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3axojotwv.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3rmgnbuvp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3zkursekq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ylmxtwkd.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ztowfjub.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pwbgewtv.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3krthlwpz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3beezngsv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3zfiiiadz.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ufoudgbu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3vxkczquv.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ltxwtvcy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3buokpwxm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3euofpmgg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3wmincgiz.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rfintvmp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3yicjdkeq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3rdlpjikt.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3zjwidxsh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3snxrocjg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3zaxwvxfg.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ogldxkzb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3lsxuqzef.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ttlzcleh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3yghfyjov.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3fdeyfuxv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3suswcsax.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3cbvembpm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3birihjjp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qnvwlcdm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3hbztdsdr.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3xpqazanq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3nkikptyq.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3pipulmjj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3sytncxmk.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3hmjwygdy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3hyyvzlvi.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3vdhbajap.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3owrhswrq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3kqqptptx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3nqyoylwu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ygbvgysf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3zcpthysl.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3wvchlfzf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3twmsphkw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mjdfjrkh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3tcgucvtt.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3eqtvqshe.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3eqzelegu.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3liizjond.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vhouwyvz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3bkvodfqq.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ozdjblhi.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ceaxglby.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3tsvzyrxc.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3drfbtwol.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3umkncjpl.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3teotjgur.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3vrollzvy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hqphziba.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3bnmhstvx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjtkopxt.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xtgmyfdo.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ttcczcwr.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3kgkzmzfk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3edjirtpj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3mnqwowdb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3bquteznm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3dglacnnq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fzwzpnis.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3irhgjjsw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pvrxnsnt.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3kdvvlqqg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3wittawmo.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3fhulhmnp.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jkorccxj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3zeyuyhqc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3cqndjenl.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3pvvffgmi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pyfyynyq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ppnmjavf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3hmxyjcos.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3tckbqccw.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3bjzafwmc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3qpaovtym.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3gpinivvp.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3wfxueqrc.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3czhvmrmt.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ositmpaw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3raqgacvq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3mjwfkopa.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3udvovdew.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pncikccp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3octicngt.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pjqsxeyk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3jhysucbi.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3irwacqqb.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3pghnhjul.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3caxniwvt.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3ssrxysep.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gsudaiok.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3pbohqwup.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3jgryefty.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3tmancuqn.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3lxczlysv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3xusbmfrm.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3vzwupain.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3xrphuwbw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kngfxdwj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3yknalgku.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3xegjmeyf.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3bubeibru.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3rwuvsunt.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3gerqobbd.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bmumdzqh.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3qjyzgcbf.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3taccjymt.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ehalfaag.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3uwefiqff.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3bwxiumzj.html


<!-- 参考信息 -->