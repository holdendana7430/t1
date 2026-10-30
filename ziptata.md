代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gglzzjvsn.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/guerzdweu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gmzhoqmao.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpqphztz.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/grvptlxxx.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/ggktclton.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gxveonpbx.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjsbbmgi.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gzyfqanxa.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gauaaqmyx.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gotjpdqxf.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gpyykokfs.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxrrrizj.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gielgevns.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gnpuafoce.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmrpqmpem.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gxfvdodth.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvfuvefd.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gbflxhwbk.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/ghugqptkn.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/ghnupqcug.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsxqahow.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gvcfxjxjc.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsucujgt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvezvxbi.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gjtwfxelx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjctztlf.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwguaigq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmgtxpui.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpkakxoh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbypftxk.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gbpwnbojl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnxlqkss.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwqsobvz.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzjyrjmb.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gmcwkjhvw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gvwcgehzh.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcyakrqd.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/geqkcsccm.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/grfzeszuh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gsuqhleap.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdqadptx.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxdvitzr.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmjibrux.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcsvuwcy.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsfzgssi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/ghrmysarw.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxvmbueg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagyyawxl.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/glflmmqfr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gsugmrdlk.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjmksevx.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/ggguunqyl.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbytuyarq.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gxownkmft.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gnphoqeye.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/grrdojsxf.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gybebsjbn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gxaazzxgq.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gzkcwgmol.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gjvorhupc.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gqppwddqk.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfuyqeby.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gqrbxdmid.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gtcugwfjw.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gendlwtrs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuzhwwhx.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxnjvtfz.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnrfdscb.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/geexirpwi.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gremloxdf.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gfijjmuia.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gntkxvudp.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqexgcww.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geitiioaf.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gijrvrcko.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdjjbxtq.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gsfegdomp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gatvsfuke.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdmhsmpm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gxnikrump.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/goabgumsi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gewvvkysc.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gcrxjqyrh.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwxjlwbs.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyvobfyg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/glwauhpun.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxjeqmyj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghjkegqem.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/ghylhgmbq.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gelzxuust.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gftelvycw.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gxswwaaau.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsprdleu.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/givfmucdp.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/glifilxtc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdvrbcjol.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmrawalx.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/guklumwmi.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzszksrct.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gnqffyxly.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gbmgrwqqa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuwwtdbx.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/glzzqoyyq.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkbclraj.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gwdxbjpdn.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gatpzzajt.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gohekqvbp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnpppccx.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gmisasiby.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guemeqchu.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbcwpjek.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/giubmzooy.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gftioxjlx.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gumgzfdgi.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gduowvnkn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gyzdhhyji.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwadnptrt.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhmppaqm.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gjowvnclv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gywrnxfyt.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gohluvhwu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvtqhoxq.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gomnaqnni.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzcsjsev.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdpnhubb.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gvcnyqjew.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gvvysxkkf.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljazhsyz.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/golmelgkz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gokommnkn.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gwomqzcbz.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmihminfe.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/grbppaace.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/goqpdkrdl.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/geiksmmzd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnhuwhsw.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqxojltb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gpebonqbz.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/giqddzuzq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gnakvvlud.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gdpuhxhlp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gfgoxxqxb.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gtoaqgvbk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gqjjguptk.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/grfniahui.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gltqwnbfn.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gdukbiqpd.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gjuitemak.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/grnwysibs.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gjrlbpivy.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobfqdqxc.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gdnmfrpdf.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gruxexbgl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/ghkzqlqbt.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gopwbllzf.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gmzwbuqay.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/guhivsyjz.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gqcdwvizb.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gvbqpdjpz.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gfvficlsk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwrfpeese.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gginkbvbn.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkegsbpa.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/goouhwksk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gnkykxwcz.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gogblases.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gijcqcwfs.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/geazvpwhp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekhfxzvn.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdbdvbjv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/grvjwxlyp.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gipoxbamx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmxqtsfj.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gshrbazhk.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gzofezjux.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gqegrhfzw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gjurkjxbf.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/glxukvnge.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtoiweod.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcksmejev.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gywfjfeyn.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtlmapavj.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlyokysk.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gffnyvrue.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gglutdocg.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gtftsrjla.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gctmhtlbx.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gbthzvxol.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/glsyaakcd.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnsgfbto.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccqdbitj.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gglzymaqa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxdemntzm.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcsggbmhy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gybbbempj.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxpbyaae.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmerbhfv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gjwjdwcbr.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmhcugbk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtptuuwt.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrgfnzbu.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzbagfnl.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gavvcvjtq.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtgxdmcer.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrknjwaj.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/graqxjuxm.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gcbncbidx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/geqdvyrlu.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gargspdjx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geueclloy.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gzskkhwhv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsxyzbdd.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlugyznc.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gcixlrdll.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjjgsxwk.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxwvlcab.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gidwavopd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjqrrpzl.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcffaitj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gaakskqli.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxbvhyxoo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gdymcytxy.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gypwxpmnl.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gxigltqeo.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbdlauqq.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gndcubuxh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezemsktj.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gzmoibtmz.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gryhnlmng.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/ggzkpzwhw.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gjlgvffzk.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gnnevkjob.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/geqzomaem.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/ggufakknd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/ghkvzdwfy.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gpejdzlhz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/golqlbhoe.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gstqhgmkx.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gqbkcnuut.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/goymupxnw.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqurfrap.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gnmnyodrl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gxqtwajae.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gpbcgycwj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsycbnfwu.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gkfezgbsy.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjyuiovd.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gzzxkrzyt.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gemnslsda.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdqpgbuo.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzhtweoy.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gcygknhle.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxwzttob.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gervjltih.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzmzjedd.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gkjbzioro.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gnpihmvkl.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/guttmtsos.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhqznncn.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gairscuov.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gqhriyqyu.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmopvduaf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcxdldjl.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjydxugd.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gqaxaxwip.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtojambo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gutqzkkjd.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gwjidpslf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gcldfpgwb.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gtdeesccq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxhqmyci.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gunliylzl.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvycplsjb.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gxdwqfevp.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhuisqor.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gypcptflt.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvxgyncp.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gjoskdhku.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/ghkjqyyhq.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/glzbaymqz.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gvvjrmwjl.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjwtcmmc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goytikkin.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gibamflih.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjqjxcag.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgooextl.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gllbvsfzi.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gpuyuxpov.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqkeciwh.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtnvxfyw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fanxiaobao.xyz/Article/details/gtemkvwxw.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfwlamlm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/grcblhotj.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gavvsjzeb.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/goxoeimee.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gksdbrent.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjjmfwpj.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gbmbiirms.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gdqovsdug.sHtML


<!-- 参考信息 -->