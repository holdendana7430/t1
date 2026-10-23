代发 wailian999

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3rigqrwuy.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3irgkrmuu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xhozauzw.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mxkdoteh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3tftfzudl.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3snfiiycb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3dphuqwap.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3hialyvgt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3xfgbrxch.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ryvsqfvc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zekkbjqy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3rdjpclcc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3kmtmxiac.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3xoerbkvx.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3zszvfdoz.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3igcjxshw.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3fmnqxkuc.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3pvbplzzs.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3tkwuuloh.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3yrfjfgus.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3bawyqgku.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rdrnshtp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3mplqwkki.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3vuvvfiui.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3bkbsrupi.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3odkcsjwn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlesmnrh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3mtfxtbzq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3wqrlpptp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ardqwusq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wzfajfey.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3eapyggjq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3hlyslugo.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3vnmvecuw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3lghrubmy.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3mgirmcob.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3kbttcqqe.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3oujfsjme.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3vuknkvxz.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3nvcjaygs.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wloijetz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3utpycyqk.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ihkedeny.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3xxslaqfz.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3fludgrvs.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3mcqxcnrk.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3zwfecvbi.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3gkuatjbg.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wzuiqaox.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3jmxwebjx.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3rstsamez.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3pnuozhcu.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3giulhctp.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3elitywqd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3lmadxujg.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ttxvtixh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kjqfyxnn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3fsiabcao.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qhpupler.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3zdxtmmaz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3orqjwqfy.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3engbsmku.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fiokgxxh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ncbjgjan.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3hzgcbass.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3sxbjxrjv.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jafatifu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ncywqxuz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3wlsrqbim.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3bkhlnrmn.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hcumxidl.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3larkogoh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3egkosjfe.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ffzjxtzy.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3dvarruzb.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3htcnorrx.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3nrprnxmq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3hyokinps.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3norfphji.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xhxsygvq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ueyfmecy.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3yufmpsbu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3hzmatykc.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3suqrvmph.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3kshwukep.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3zhspudmh.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3zpakwieo.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ijxbcdxp.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3sochhlft.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3noumlsud.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3xfqhfmqz.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3wyyxymsq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3aqidgdqg.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3rqhkdelv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3vbctaizr.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ghyhezam.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3zamtmvwf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3oifssjps.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hosmbjne.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3gapmmnai.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ankxvpmk.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3xnjdwktz.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3tihdbrlc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bbwjmaar.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3duevxwbx.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3sjkybywu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3jqabwtop.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ghwsvgth.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3lcjbihuz.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3fyupqmeg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3dhvftsfc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wwpkpeoi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3dzmoikpu.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3txyinibv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3hikvxieo.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3oqizoufj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3oiwjqlno.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3htdxxmgg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3arjloywb.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3vtujlowx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3wwfftcev.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3joqgtosc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3xchcqfig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eysypuch.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3bywnukcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bmotnljw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zfynueof.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3yexudukz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcxuiulo.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3zomsboyj.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3dzquskox.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ijjsnoig.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3vxesygja.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3qvhwepho.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3jgyjevjp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lbzsexjc.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3oabnbzfo.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3idknrlwx.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3fxcjjkqe.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3xumhjrhy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3nqdiubne.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3njrkqvya.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3tixhysft.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3thqxzqdn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3chkxwprm.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3jasixgmk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3udyktlmz.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gglregug.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3xouxsmjk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3rwbipwri.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3isizuhnb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3mqeozkqq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xwamtbjc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3gpoezoew.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3wqvojbmn.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gipvrrns.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3edognevj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3cfbogseg.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3loseazbl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3fhgvpdva.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hyorcogo.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mgfgbxci.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3cryxpkci.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zzplgoha.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3vrqxbgvj.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3cfzpzjpf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gijqikyo.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3kkgktyei.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3lkcumxhc.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3hdctfxir.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3wcetjxql.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3hjianfjg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3wduospia.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ztexntjt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wlntrwkf.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3yizdmnwi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3jasfhbxr.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jekculnr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3jjbodrnk.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3igvrxadj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3rcnftteu.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3zqemypqd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ythvarbc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3kllpkfwf.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3fugutxbh.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3saoicgdj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3zzwhbebc.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3mkrsualm.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3yletfnjw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3wbasvtva.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ywjaivxr.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3srlexqdr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3qpjcfdxk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3icebxfaf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3iofhshdc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3flaftbyf.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3nepgqtyw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3iuvymiht.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3xxpbsjqg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3vmlxsghb.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3psmegooa.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nxjdnqsy.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3hziibaxv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mevzpmnd.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3tqqcjovr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nmogwbhj.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3vnlxsmxm.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3llfwputu.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3sxcwsask.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3rcdalaep.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3qdbohkvs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fsdsueid.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3jqmaesft.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3xjdymlrx.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3kdlvcqoq.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3bxubwyro.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3tvitlylb.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3vxclabhw.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3gggifuyt.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3usserjii.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3dufyoicw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3tvtmgliy.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3hlivhzup.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3cyuxytwu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qutfgosf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvczxfjn.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fdxrgvaj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3cgjwylox.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kyryfxwd.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3cmzkhymz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3lerufsdv.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3qyckkpwm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hpydtowr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3uklexlrm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3wvvshrkj.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3bkjwzirm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3oylrzcil.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3abdrytli.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3uguykork.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3tdbczvof.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gnqrughd.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3zuwavvuw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bmvtpkeh.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3sckvolof.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwwcudgu.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3izbclihd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3fvofzwad.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3uqxyfoul.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3fuioghcp.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3xrqpjvbh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3yxwzaqho.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3hqoiyezr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3hklbhnoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pejxnuus.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3aqgawztt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dpzgbkid.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3aypsdcqk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wdyfagir.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ssphttns.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3lfrlnndj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3zdeclpxd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zasvmaoo.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3quhtlhbj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ywuwmmvl.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ubepkoca.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3wfgsfhiq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ycfuqrtm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vwyexdne.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3dhiddmgs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3tjwoemtn.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ltglrmbj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ldtjvulp.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3hgeslwdp.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3pobhezlb.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ncyffevh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3iginpoip.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3onpriyqc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3mhcytayy.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3dmkgbklq.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fvutexak.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3bmmitqob.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3facuexsi.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3jyefqnvx.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3khmpdmuv.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3gditqodg.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3fzzhbdxw.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zrhuwxfg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wzhbmxff.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3nhfzxvnl.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3yitdmptf.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3npxrtjrx.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3mtuwlpkz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3norchiwo.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ujrkooff.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3gwfryopr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3yrzrwfci.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3nuaoglev.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3tetphvou.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ftnbrjff.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3lzclzepc.html


<!-- 参考信息 -->