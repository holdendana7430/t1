代发 wailian999

esac
来源：http://www.52xcode.cn/Article/details/gt3givlzgso.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3beubfvav.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gqahkrxt.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3rbzrubxe.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jbasdtqd.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3abmylcov.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ovmyvlbc.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3sqhejepy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tecwijvu.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3uwkzcuzt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3llgsinpd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3ydotzppg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ksnbhuwm.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3msofdvho.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3mwvkpfzs.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3wzzniest.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3jejutrxr.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3oxrjiecp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3yuzzrtlx.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3plzaosha.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3dfrixkmr.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3rthwirye.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3irmpqoqs.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3shrqeken.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3chmalsjs.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jujdmgjx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3watcklul.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3cbnylaub.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3cdwmivuu.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3wpssttfx.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3iuwvvreo.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3pfngkfra.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3agpuuhxb.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3jjfpvvhk.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3rhcvbmij.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qmxmabop.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3opnagsrw.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3aufegggp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3bzcndbbh.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kziagfrj.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3mokqmfrh.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3xsovqimh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3srzmuith.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3mouglsoq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3patnsrdv.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3groghjgm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3vincutoe.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3yfzmjtne.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3vvhgnxzj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3lskmdqeb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3nwqnfyri.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3tzxjmgys.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3pxmbvijy.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3kzuenrgl.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3utpyyvaw.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3cruamodr.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3evfoamvn.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ictdhvdg.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3vzpvfwut.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ergawgqa.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hbhkoaom.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3dmelzksg.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qpsudebr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3srkxtydp.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3lsuljlal.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3xkqcdwvy.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3unydgoia.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ykqutnla.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3xzkbwhwm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3bhmlnjwf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ixhcmiwc.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3jpkobjqf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dmdnpodl.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3kaqfyavh.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zwecissc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ngbeumou.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3wxrrlqeb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3bwpsvycn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eaohawps.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3diysgubc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3lfsdprse.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3kbdjzmqe.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xynquocl.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3cpkvqjmn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3pkwjsplb.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3xxhbexbd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dlryckua.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3yipfkpwr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ekqcuhls.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ljfmjkzy.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3moebmfvf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3vfosgzcv.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3pozcofgr.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3upoghxde.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3xtlcnxyc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3rxiawbmw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3lmjsryja.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3uhtmilfz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3mydvkkhq.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3dhuasxqh.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ktluzmhq.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3iiylsnue.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3sxatnvcv.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3yfawmiep.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3htadwuuc.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3imedgrye.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3gcehwfrl.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3dajlphui.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3miwovbtn.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3fmblkapv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ofxgoosc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3xxalcllr.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3tiyjidmj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3zbptkiyc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xisizsbr.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3niflknoh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3zeceyyjs.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3vendxeyc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3gvzqlzak.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zjkbmmnh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3taxlpjon.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3hlmyhfpv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3awsdwomi.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3bwdscngv.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3piippnvy.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3frxkwtqt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ewekustq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3pdswpwip.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3zsrqpayk.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3otjkenvq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3iwqfneeg.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3zkgugpng.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3jgwdkxjd.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3dpqekagv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3pwonnfnz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ihjlmkqg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3wdbrqlbk.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ecobkptu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3yuvuqphm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jkrgeswp.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qbxcxksl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3thtrwxms.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pxaclrgc.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3iyeqwprc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3jgticdis.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3pooaghlo.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3kqqpzzrl.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3axfywtop.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3rgwtkwij.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3jwuqjcbo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3qrkvcygq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jmzmczem.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3dbynzowt.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3arueidyr.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3pyvbcvti.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3azfpqkur.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3zgekkity.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3nqnhdwll.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ntzavyhd.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3zfnxuplw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3nerqiccy.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3zqrgpbjd.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3kjjsejlh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vlwwbayp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3tahnomes.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bgowlnro.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jdtoknnv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jektfgzi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3syazrypl.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3nfmzhiop.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3dyrvethb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3kgqwmrsz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3kfnkyghv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zmddzusz.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ruiuudxc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3nrpacsex.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rxjrdrzr.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pmmagnkr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3isxxhbuk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vgpliiwp.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ybmexhzi.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3bmtbspff.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ebltngsb.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3fyfvyfmq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3kmzcitiz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3cpmtyczx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ddopvqhh.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3slgsopwt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3zfqokegh.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3rkejpcbq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3cdpkweqj.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3warxkyet.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3cebegyqy.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3oluuygog.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3zrroirbu.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ltzaeaob.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3iddrwbjz.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3niankkra.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3undjhymj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3evvmezdg.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3pahsyxiw.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3eaaqehbz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3hggjvznt.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ulhcqyod.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3vyojcoqu.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3jaqynnkp.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3pkjijhxh.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3reqrlqpd.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3uxsgefba.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3exnmjiza.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vqiuimdj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ebbhegrx.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3jpcjyoux.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3jmjwjwih.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3skihpgoj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccbzwmqr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ufbestoo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vczkwmjc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3tbkxpxsj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zgjeltiw.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3gmdjlzxt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3junbvjtu.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3nnlscefg.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ektmeoak.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3hhgqbwzb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3gsgymejb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3khtjuskp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sppjpzme.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3raxkglno.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3nfqkyolj.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3zjupntyp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3khevpkzu.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3fqhxgdhk.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ywejiysp.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3chgkogwy.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvcuxjzo.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3kgxiyega.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3dqsazctu.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3xekznian.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3vakasspm.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3eqcudqda.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3kwinaexg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nfgkggge.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3mjygdefu.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3iipilpmr.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3mcpqcark.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wbtsmeap.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3vvylfchr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vtalkqok.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3agtuvkmh.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3sebkfmdo.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3mqvculko.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3vdgtskly.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3gxzqmaek.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3cowwluqd.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ejbbafkv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ctducevz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3uezndbue.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3wjrdnvqv.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3lokiamlq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3xliwifmp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3injlxdod.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pbhgdcls.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3nhszpmzc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3lzivitpk.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3fgbkzhvw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3enzymrsr.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3shrffkgz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3pspjqhic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ickhfhfg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3wykbosjy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jeptogrq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cykxnyjg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hhzcznjh.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3wlbmwhlm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3bobseykh.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3kcyjxldo.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jonltxfr.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3pihdrfiu.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3iofuaqau.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jbdhtxdo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3jselqkhv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3dqxojrmv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3amwgbjyq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3hpguocks.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ljmtrhhg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3fmlomcte.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3eowmwsny.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3cortakzj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3qvqlfuuh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ykiwsorl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3amgikdsm.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3rlbgcuml.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3szhuarsx.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3gpnpxerx.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vqcfnfpl.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3fpnyiprz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jzjspwpq.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gzzmcsyv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3nyunwxnb.html


<!-- 参考信息 -->