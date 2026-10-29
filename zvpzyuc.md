代发 wailian999

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gykzredcn.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gtjponbnw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gbgyygouj.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gzbwmkxtm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gulqkmepq.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gpdxmytcp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gfepywnfs.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gevpmeppj.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gavejkwye.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gmwzyoied.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gyaeychyb.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/guqatdkfd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gnqmnyvki.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gnqkacryk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gewxyxnhv.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gkgpuaioi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gpdjykhab.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gigyaysxq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gmjxpwkfu.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gaocpdqhh.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/ggjhwurke.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/ganguvuzd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/grofviegv.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gyylcumsq.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/grwkmmjjd.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gqdriueca.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gydkomhiw.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gkkdqfzbw.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gdwrbqwqa.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gvimjrthb.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/ghcnkkxtu.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gergzndlu.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/ghuvgglan.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gjlrlbozg.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gcddfcrlc.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gecocfucd.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gmbqkfrro.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gosftminw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gjcatuhps.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gyfljrqcw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gpycgvmct.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/glogypbac.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gwroarmos.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gxencoznn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/ggicjpmjd.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gnhcyjlmz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/guviiycej.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gacehqsiz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gzlccfwxb.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gsylrlkry.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/grbisvgqx.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gdmdacxgf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gqogcxfgq.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/genonmigm.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gkgtoadiz.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gbphitxow.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/giwqkscex.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gidpgzgtu.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/giomzuiyr.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/grgbqrxhf.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gycoewegn.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gxjjtkmvm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gyvxmavni.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gpgtahdhe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gvlgcagrh.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gkxjcpuoe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gyttiirwi.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gfjklmvcg.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/grczuselx.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gejvbqweo.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gnsrbqzkg.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gipgccoof.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gobubheso.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/glopuxmsn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/ggplfwjsv.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gurjwtgju.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gbpvoogaw.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gxxfnhooz.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gcyaqbrmz.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gmwdkjeuo.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gipjjwhxg.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gpjglssqh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/guqtqleos.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gnkdkfbzd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gqaqvzpul.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/giirxkcek.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gnlzxglgq.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gjxrbdjtj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gwadcsrec.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/ggmzzusmi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gtejrplgk.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gnnaoqcdx.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gbaynwmyw.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gykiiwqjz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/goinddqtr.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gebsraurb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gkebndwcn.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/glbyqvjyv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gcvksqxiq.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gdnlhxofa.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/ghqvhmkkm.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gruqhjwkj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gfjnngcfq.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gekkdoned.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gimhaefoi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/gjovamusb.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/ghzeypgvh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gilzhuzyc.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gwjhvannv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqofcjwni.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/ggrlfxvnk.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gudkmwpzk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gcatutsfx.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/ggzrehsam.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gtdutmgnp.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gnrogwwxp.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gqchclyog.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gkrfmpowh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gxguangth.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gcjxvoucj.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gkfoxkhvn.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gbbrxvkjv.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gkdtodegd.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/glquqhkbk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/ghpgekdzc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gidjubavr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gyjnijcma.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gvpydigms.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gybiulrcz.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gixxkmird.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/glhmybezi.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gohffshgv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gjlyniuyj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gxsvpcksl.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gzkjgvgpf.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gzrwxafdm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gyetcekla.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gqkxdoekm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gxlhtkrig.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/ghiqrgnjn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gmewidxai.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/ggmgvlqds.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gfxmotmsx.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gqvbxitrf.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gojjdmkqy.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gvzbdskdy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/grglghnzw.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gpqcbycfm.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gsltgyppc.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gfliaggrq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gtcrvaoiy.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gzibsravz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/grhccqsxl.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gtzxyrlkm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gztprauok.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/grddsezib.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/geazzafdz.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gknieegwe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gfttjdduu.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gnjryhebq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/goskcvdqy.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gxlxelqoo.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/gqotdafay.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gxybzbivz.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/grttmmtgo.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/ghezzgmui.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gkylrbfmr.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gwxfpexjw.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gjdklcnio.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gcafahtxr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gtfqntycp.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gcdvuxqxi.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gawkszsvf.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gqcbbcclr.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gbknzseyp.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gktwrtlfj.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/guorixaem.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gdwivmfue.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gwnfyqinz.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gupkobgnl.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/ghfdxwejk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gnwbqujcr.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/ghznlnrgn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/glxxcssxb.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gngtanmnl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gjwbvijqj.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gpfuvaumn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gldsovgjd.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gaayfubgl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gxwxuuswo.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gfidrscqi.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gjrzgjkwy.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gichuhbwi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/ghuqvtsgf.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gnresfpcp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/glheboeko.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gdpuntnen.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gfeejvkny.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gpmtgldcx.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gesbjprmg.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gougeixzl.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gurfexbvb.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gowicnlho.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gyftnosgu.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gnewqwmyo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gxbpyzrxa.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/ggmtmznni.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqvfngswx.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gjkqqvpwo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gekiwvkpl.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gxxqpmnhe.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gkutbppvv.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/giweulbxh.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gortwykbm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gczjextqt.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gspcbrbmw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gwyyqbbqs.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gdouuezxe.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gclpvocsq.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gbmeaxgby.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gqbeznmbc.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gmgigmulv.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gtmccespi.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gdvddiygg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/guesyonsb.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gcrzdahun.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gikzwtfhc.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/goygleekt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/ggvtvrqja.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/guhcdukec.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gffryceto.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gzxocditi.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gryxleijv.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gvwhyvtji.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gniedqdqz.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gtppulofv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gewwswguw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfwzlfybe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gqeoageja.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmirmldpb.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gzjaszynq.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/giuqzbpaz.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gisfmvfmb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/ggcyygmzn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gwsnipwzt.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gyjvkzwvs.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/grywjbbbp.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gbyevemxh.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gcvnptzcr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gwldinczu.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gcujhcxqu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gsanbpuwm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/ggeymdrji.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gvyddnlzm.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gswdwpsyw.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gsoltozsm.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gywkcnogg.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gwrjqgfbd.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/ggkmxuzzs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gcuepuinc.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/glxjdlwga.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/ghxjielhd.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/ggjbxjitn.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gslvzgpbz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gukpukyrl.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gpyttbovj.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/giwxgbhhf.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/grwhiolov.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gzrfpoidb.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gkfblxxyv.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/grszbikut.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gofacnkzc.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gpimpmqme.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gbieqsxoo.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gddstxlyv.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gpacdvbkj.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gynacvqkn.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gzdvyjnuu.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gkwsfhzdo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gsplwevzn.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/glqezcoht.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/ggmhzjwoh.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gykqkrhcx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gsevuoery.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/guxonrhsi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gznfljohm.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gtkyhficu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/goefgxwii.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gxfjchfmr.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/gpohocnkd.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/gpyskzjgv.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gxhzoetsi.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gxwocmjvr.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gqovbbcyu.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gakfirlqo.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gzmthfrao.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gnlmmpdsm.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/giwpzagtt.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gqxxfdjuq.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gzivhyeyu.sHtML


<!-- 参考信息 -->