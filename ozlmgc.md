代发 wailian999

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3frpbbwlj.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3yyjsdiur.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3phkfzwsc.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3elgzbfeb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3feoqkaaf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vpazwrpp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3snsryoyu.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3stkmdqjk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3rpbdrnzz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3flzctyso.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3mredjqwc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3demlgnpp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3vmanusvv.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3wuphwxec.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3cigogqcn.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3cyhvrogf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ulrrqcck.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3dronhgax.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3fdhordzn.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jbbawdoq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwtjpzem.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3bmaxdvxp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3kewdspun.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ofywkhxn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3veudziqq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3dflduvdg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fdkhwhdu.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3jjupwrhm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3xjuqzgco.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3aepwtynw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3nyjnbwbk.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3apmitpju.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3rvkcqdiq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3nplvxrax.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3smwonptr.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3wqfwqqba.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3tvevnqme.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3zebibwzv.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3dbfbmxja.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3hjjutvsb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xtkduobm.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3knabqhrq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xqimwefw.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3blqvqthv.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3htplumyp.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ukocdatt.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3rcigklbf.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3nwtlechq.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3bopmocwr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3rhcasxlc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3jagnezca.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3qqljhdvh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vrubbzwj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3aawasblg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3sjzxdrpp.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3kveardgh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3pdmzevwy.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ffvbrean.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sqgeanod.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3tuclftem.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3mkpqkabq.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3rrsuimju.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rjnglvkc.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3libegfqo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3kgufpfiw.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3lsxuilsh.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3onyfszbw.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3jnbgkdlo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3dexmjbyx.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3hqljwbjf.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3nnlkjbwc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3rgixlvlr.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3trkziuze.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3tjkphexq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3idwmgzsu.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3rwaidtrb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3hjswrjyj.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3suulsjhg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ahbtohpb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3lktqklfl.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ayezqxwx.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3hhdcijev.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3hybhwhwl.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3tazlzqmq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3qpxqyvwj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ijfowena.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3wrthbolt.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3lcadaeba.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3lfrxoltt.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3uwvkbogc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3gksdioji.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3owgkhqtj.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3qfhlxhew.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3tlyusujg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3azkeumhe.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3lalqdiul.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3zhfxunpg.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3wuxgvlyp.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3bttpdcqw.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3kgejzbbk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3qhuuqewv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3qmfkiqgq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pftblbbf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3kyjveenf.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3jekatmou.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3smfuewxg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xfoonvmv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3gsyondds.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3xzfpntth.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3qbvxcrjs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3bnbdiova.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3yhexavqd.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3jtnjkvav.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3slwtssdo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ujopsfyp.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3nzhmcuol.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ovyirtgv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3zqjhsqqb.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3uudfoymy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3asiuizwj.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ejfeldku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zrxeggpg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gvkipwqp.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3msnrtpvu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3snqxrwda.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3vsfdbkkp.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3xritvezg.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3kdyqvpso.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ktydccvk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ahkgtcgf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3enkisuxx.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mddaihzo.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3zvxfhsql.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kmqueheu.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3pucelvuh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3kjlumkpu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3vtjijsxs.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3zvomsoet.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3wybnusmf.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3enhooska.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3omzadmob.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3vnokmzmi.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3eujkfwfe.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3blcrffia.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3atvzepwj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3munwpmqs.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vwrwystz.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3nshfcauh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3cmdhmqgq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3nbezjeso.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3aqjfgsjr.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3nckauxtg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3vxwadtha.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3okrszihq.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3zxylsfjd.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3jtssegjr.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3mkgxfazj.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3avzcqsny.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3eptjczet.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3revlanxk.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3kcdvywsl.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3odwqfamc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pztyjnzz.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3pvmgdout.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3zyccsxft.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3xcxsqugw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3cfjgrzcp.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3mzeqyibs.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3riyilbzu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3wkytbdru.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vftbhbjs.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3vrxiooxt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3lizlomov.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3eaeeozhv.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3vpelzhst.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3xhawwmif.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3usmuqkzg.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3jdopzamc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yorxbaxg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3gjtrcxsc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3mtslvqzm.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3jsjrnenk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3mnzfdqff.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3mcfspcys.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3svdwhqvy.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3bfmteift.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3nltwrzdl.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ghvaykbd.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3oqioujhw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldwrbbul.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fjtnrtjo.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3jwwscxwd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3wexzhsus.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3qqswnpij.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3wjsvkebs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfroneup.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3yrjpcgxq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xjecjxyk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3qflcoyof.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nvaomaep.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3josbfezn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3bdrbonty.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ssutelhs.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3wqnjcltr.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3cygbfrcd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3aenmaxtq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ztbtbqtk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3typozbqw.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3kdzacgef.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3uzotuqpx.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3hxlgnxye.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3txowallk.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3qngtgyxv.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3dmatnfpu.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3mbdouegg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfsxdcbb.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3unfzrulv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3dwjbfzae.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3kvaorktr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3smooaiio.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3kffgmxgp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3jvgxjsdn.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kkwrqnhk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3dwndsuku.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3nstqvtqv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3brcqzptm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3excsibpr.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3acvcpjgc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gcorlgyh.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3kolpqtny.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3vdsdcjjz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ngyysfpr.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifhkoyvy.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3asmebket.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3fsdsplod.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3pkjbzbac.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ozlzxarn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3fxirwgzr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3lfrvszow.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3pufxctgk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ealpktpm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3mcsmvhzg.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3dbodmcif.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3dvytifoi.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3mwwtoyuj.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3xlhwxvuw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ivuxxkzz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3abfwpixl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rvtgywcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xukrtkcg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3jrnsqskn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bkxiduvl.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uvsqwhue.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3sgkblssv.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ddqlmenz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3yywqjmjz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3wrqimvym.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3mylkibdw.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3zwhvjymb.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3eqclkjyw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ppsorepb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3tjwvtqnd.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3kmzlxkbx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3khjharlr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3rypvgnzf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3kzximzqv.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vtcdqqvf.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3nsefcydh.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3hwgdqque.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3qqlrwvyy.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zkcrtnwm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3yerfdqiw.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3kgrekpft.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3zlgflneg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3psclufwu.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jmecdxqm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3jccxukwp.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hpnbwkrr.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3nmqrcohy.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3obwbsxkw.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3eburbwxm.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3haaglppl.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iwnnalmi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3oaxzmifk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3qpspxfie.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3goqrkqau.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fcdoamvi.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3caftxuzn.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3fysgszhg.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3zcupscnp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3tgxicffg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3konxiofj.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3mutkgfzr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3xzbpwybh.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ixqcsgcw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3umbkwbdv.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3remldgdu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hnughizq.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3bdztldwv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qpmvzpdy.html


<!-- 参考信息 -->