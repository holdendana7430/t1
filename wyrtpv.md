代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3xtjsampe.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3fmtfhewb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3kjaiudrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mtkyxhyw.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3elmgkbbq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lwnlizdk.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3jpcdhhrl.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3gmgmbarh.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3licrlccy.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3hcbghdlw.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3gfvonihe.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3qaypjwhc.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3bniamjbw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3xybjnqkd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3wkjpupzv.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3yfbkjama.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3nrjvgopf.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3whaxtmvg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkylrkdj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3yazlowkk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3onvsmvet.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3yylwquay.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fhiywjil.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3iqztudli.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qvolpjin.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tmyjmwmd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3atfzaibh.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ziutvgov.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3gmkitpnr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pwapbtyg.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3iipvpqsp.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3dktrvikj.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3edvqvfeu.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3dlkeyhiu.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wmchcoiw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3kixdqgxt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3pzuwbhse.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ekhyequz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cxpgppbk.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zoyeuhwm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3infugauz.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3tzypogwd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qznoprbq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ghpxgvni.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3dviyyaif.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ruuikere.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ozzejjbg.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xcmnqnpe.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qxynsmum.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ykmjziqa.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3tvmjihon.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3itnbupac.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3xymkdqmg.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3amgysrkb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3syuwqmli.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3mqpakrxi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3thjwlnrn.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jxjnswcc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3hjyhtouf.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3wwymunwh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3apsdqoqb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3loxgkbax.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3idqjkbro.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3jeesbosp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3vhefdnnm.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3xlbdifkb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3bhgclbjn.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3xaatqraz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3icxqjkag.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3cajzhyil.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3vspoyjic.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3pnbckvxy.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3vgedyato.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3zyflhjqz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcglhlfp.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3jykoehhe.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3uyyhaovf.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3jybomfql.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3vspyyigk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3nyqidnit.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3uftxgvez.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3hguoznzj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3gqgqzrla.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3xgsnznom.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3qutrbcrn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3clidrjrf.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3hucsiatv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ncjsrutv.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jhhvvncl.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3oihnnevt.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3hwasuqvc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3vjalyqyt.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hfcmisyd.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3daddigny.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hcqwanzi.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3pdujadaw.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3eobrlahx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3yytclkhk.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3oihkkymk.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3jtoehfyw.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3iwioplnc.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3sdmzpxrk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3jliguhvv.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3cvoippkx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3atzgcroe.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xggeqhno.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vmzzgbpo.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ymooripy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3wmwwtnwn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3rlpzapca.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3talnyhbn.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3gyrygmda.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3fnoegdls.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3fhsytbzt.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mgyvumzz.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3vmkuwrlw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3qeseolpe.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3hlihnwav.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3iseazxlu.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3czepsaei.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3rapkvnwn.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3szmssaax.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3wcoqeuom.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3hbykuhem.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3uwqheuwa.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3gfmzkzex.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3tihnkmqf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3kqgjzbti.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3wksodjoj.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3gqlyjwsc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3jjpkcbet.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3hauqokrh.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3nkoyxgfv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3aggwoqvy.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3yadpuauo.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3tmxbhopy.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3mztocjwb.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3wvovhaig.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3omjixhrr.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3qkcfcxxr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3duxbigir.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3fkxopqnn.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3xkatbobr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3wlpgehkg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3cdurpaje.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3dceuyfes.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3iehetzlv.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3vqhkyxys.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3dycstoao.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3dlchslht.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3pqlzdarn.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3muehgxod.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3getqhrfh.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3mscaffci.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3qjrpntfw.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3qbtrrgaa.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3jfoaifjc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3gpnkflfi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3icfblnph.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3zacojslp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3nudreaju.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3jrfozuhe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zwjlvwih.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3xyteafyw.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3jdtfhldw.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3osqjaigq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3zkpizneg.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3acwacwea.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ltxwwlxt.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3jxhgkeqf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3onuqjlda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xqbhfocv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qqzszpjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sbwhfjrz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tlyxbufg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3rcalddcw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3jcpsuzsv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3bfxrobau.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ydpddqhm.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3hzllyvwb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3bvydwmfn.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3sjthokfo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dkrhqsfl.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dshkjgtx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3biitpagb.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3junlhuiq.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3msomcopb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3feenowbl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3fnygqero.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3wkkzppia.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ysmexrqg.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3pqsgepoy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3uotpjkdo.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3hezhynuw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jotpnpgw.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pslvajbl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3hcuwcfil.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mevdoest.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3hbshsycl.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3nrnhpvgz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3tuixxlyu.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3wvoknmjc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3vquidgum.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hzwxudci.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3vjncirwx.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3spkfilsl.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3loxoutct.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3hiwvroji.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3reybygxh.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qsxohctn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3doaamdtn.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3cnlcjomo.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3vhvnxqla.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3roxjqrmz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3fdzuhbkv.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3dlxalqjo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mgqgvcqp.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3zoytguqp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3lloyvccn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3iguyoloi.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ejyorkag.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3lvlkbmkb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3phufglmp.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3nmfzyija.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3jussqtve.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3isariltg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3caqmbtas.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3fxvkvaaa.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3mddxgjyj.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3dzbekjfg.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ntpelmut.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3urpidmjw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3oicgxgzn.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3kwhxwagn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3jxajpipk.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ppvjgwxm.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ydyzifis.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ajmghhuu.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3mpyndiso.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fydhuqqz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ejzgthdt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkdxzwui.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xedkyrsg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3vcwsxbla.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3hycvuttf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zkfjgvii.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3tntzztzd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3hybgizkk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3apmtnuqk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bsrzlgnk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3gvctseet.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3meokidci.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3hkfyplky.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fyskcztt.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3xjqyicfc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3gnkbldst.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ubnaorbn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3wkogewzg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3jxdcnlyi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ntnamsuo.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3llkqrmui.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3tgnirqsi.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3rudidzbq.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ywqookdp.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3dismzsac.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3hnroggml.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3kqxqdfkb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3vpnjxgml.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3jpqazvbk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3cazwolyk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3bselbzow.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3mcahvqpm.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ytvbnasf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3diodlbyz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ihvbvrqu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ortxqeqs.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sjvibgxu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3rouswuqf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wioavkdg.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3vldhpdbm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wgphduqb.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3tfqgwskp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3mzkghkpr.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ikhihsho.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlslzrqf.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3wvxgbjqf.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3hbgbctsv.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3lsebiymt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ludoqmic.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3irxratdn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3obihrzaw.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3viyemppi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxybbrtb.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3xeymsnac.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ldanltre.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3kvfrwjhx.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fumvzhyc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3avgmedsy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3vvnmxcal.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3qtskvknc.html


<!-- 参考信息 -->