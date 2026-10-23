代发 wailian999

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3upekgscc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3htorownb.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3xsqbwsgh.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3foqdzctz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3truzoxbx.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3fbserlpl.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ntunacyk.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3gyfohypr.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3fyppzwsc.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3xwesnvrl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3pzunkadl.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3lrwhxdxs.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3dzovpyid.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gvkxrseq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3izdoaips.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3gwezeqzo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cukcqeea.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3rdpckmiy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3oeshanxy.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3sydvbvfo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tcuakfxk.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3guaikguv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3prspseyg.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3dlyhkhcm.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3guifkjro.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3vomcvkem.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3nqgomlss.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zlsgzajs.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3fjzmyqaj.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3vbilzwjt.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uqnbzzib.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3udxrmlef.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jdocqbet.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3iyjygeka.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3wrnnbhte.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hbvffpxk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zzrstsde.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3xvljxjcz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3lmcghvao.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3mmmicxwy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ilidfccd.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3jcuutuag.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3rhkigrmu.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3edkvgzwz.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ijpyutdt.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3kphpyijs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mtyojhrc.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bnlljmfu.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3tgkfxdjy.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3zaxxpsfe.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3kenfuxjx.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ejppfkir.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3nutrjodj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ppbkqywx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3moytkmuz.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3upfieulu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3otvxltgy.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3sgpstxmr.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3swlyznfl.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3lwbhnazp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ecxgkycl.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3euyzwtmt.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3nswpersg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3roifvdri.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3vxirdctk.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ufuremdq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3bcblpvyr.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3dnflledz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3dwsfzcuw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3xdvnszuu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiywmkku.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3digptskg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3phbatnww.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3hswgsjtj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3cmovwihp.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3bbubmgjv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3apnqbrfr.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3udxnktyx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3kcdiyphb.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3cwnigszb.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3macqfxyo.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3qthgqkqg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3xdnvnezh.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3eogacmdw.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3msslekme.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ruldveog.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3kniikkap.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ojrruope.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3njkwtrpd.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3siweostp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jzwqhyuq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3piofvkre.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3xdmulofn.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3dzeuuaus.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jfnivaoj.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3zznlyecj.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3jruzkwyj.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3qkqhizej.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3sgepjzog.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3rbmudyap.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kecjpwmq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3dpnhacjk.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3oiblpmmp.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3gvilkgiz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3zftmkldt.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3btjagqmf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ehmkxjlw.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3kzmhbbwy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3qfskinja.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ygmnooms.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3mbaqmonf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3rcsrzscg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3qxemwwzn.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3begtnixd.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3zondsqqi.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3kuqmqqgx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3uhwcdvrx.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ueevtnir.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3njuprjxt.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3qlbhopvr.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3qkrnrtdq.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3kitnrany.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3xduuonbm.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3itvwbrmp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3dwzkwgmv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ahjiulsc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3piniwxhq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3reffadby.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3izlrvtdx.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3sfwjkzwz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3vvgwglue.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3fzuorync.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3qxktwmbi.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3elobpalv.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3jqnsfeax.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3msngqdya.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3qluibuyx.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3jybkufqj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3mcwbzbbn.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3hraqrrus.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3jfvjuanv.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3nrwdpaal.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sjozzyhc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3bpihagyb.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3vacbcnul.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ukzjqchc.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3uuzltijv.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hfxjqfhw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3kcfdobqe.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3fqbhhwlq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3frtmkwgk.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3fwduhgrs.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3nslyoxsn.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3bxsilhmp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3wotjtdpy.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3yjkujyzr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3fpmwfwwy.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ftplsmlk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3lvjvklkc.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3nfskkgrk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ddgngjbc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3coipxweh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3vkvduhor.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3lomshtyz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3xlfvatkv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ckaknrew.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3kdrszizy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fyuqrclq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3yuassvau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lackdekl.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3shllbpqn.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3jumndgun.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3mznqizva.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3zybozmff.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3lmhdwhlt.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3tqegmecf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ofwsxclk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3zaqjtwah.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3xkakksob.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ykttaqxk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3bzcavxej.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3sprdhujr.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3exmetqza.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3pfbkesay.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3lgkehiai.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3zafrstid.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3uplltlvw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3lvxukkzl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3rlhqxczy.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3vozytacz.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ekafxlek.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tskqmqku.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3dpqnkhve.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3xqnpobpa.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3apyatuij.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3murgnbwr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3oiepbrat.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3xvvdqxts.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3xkqqyesf.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3epunldvf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3pgyqshwf.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3knzzwjkm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3gqusqyru.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3huekqsjs.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cjwyxwup.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vcacpper.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3nfnglfvq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ypdlbjne.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3scmcrtge.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3qnsskemf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3myxqwiww.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ikrupaep.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3sdsfzall.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3thsmknez.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3tdxmqsoj.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ldniuyky.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3hbiuoqjg.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3spcnjzqw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3fjlmwhvp.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3hychllne.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3jjwyogul.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bynuxhkq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ljawpiaa.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3fvuwyuvq.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3woxdzklb.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3hljyfnzy.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3klosgtrw.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3glorwqqr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ehduufer.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ysszsqfv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3sosgtmoc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ggmuqxxr.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zwwkengz.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3tskgoiqs.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3ncyqwmdv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kqqeldks.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3khpzpkpz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3lebzaqtb.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3qrkxjvgt.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3klijludi.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ypnplmjg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3zzwaadlv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3xoecvasc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3cepgjjxv.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3yhmioylm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bdddautz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3qcqueyty.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3odwxtlbf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3tfbughxs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rbpizzsc.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3gockahiq.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3qruyuzwm.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3vaghjbzx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3isbtzqmr.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3gdkdcdwn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3utcndnuf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3febcsxhh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3pgnntfvg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3xrqhvshx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ngiwwhyd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3nivuapnf.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3lzflibmm.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ctryoepo.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3zexcloon.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xlkxgvbl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3pdsbycfj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3pyeswgkf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3fhzwqxtr.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3nrhqzjta.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrneweaw.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3sjffsaid.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3lbbmnakn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3foauudef.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jtvctnmp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zergmeat.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3lbarewis.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3oqmraeiw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3dsjtvhkj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3magqwmaj.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3tfyedgbj.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ycwjnqdv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3cdohfcyc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3drsvkdzk.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3bdidzjch.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3txbkezmq.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3atjgegah.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ljdvaaus.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3arkexntw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3hoejqkcx.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3gjbyjsvy.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3kwbpzwhj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3pxwjtins.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rubpaiui.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3tkmwpmrn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3gwefsrid.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3iopbfkuc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3iikymesf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ylootlbi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ybbqkido.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eliclasr.html


<!-- 参考信息 -->