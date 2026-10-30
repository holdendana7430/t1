代发 wailian999

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuyobfys.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/ghsdziyul.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gxabgitcb.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gzokygiak.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gggfqvrgz.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjrhteks.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gcnwrymgt.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gwbzabtgp.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gonjqhkei.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/guhevkqzl.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gfthrrcru.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdaoqxmlv.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gwbmgiqhg.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gkrkgszpr.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gofnhslxa.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gmavftuvd.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gicocyqxh.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/ggvweedrp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbzdvgjr.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gaojhixoi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyltdrskg.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/guhjwbyts.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gdzgojtwz.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnweresr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/ghwpvtlic.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezlacwfu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsxhksoh.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gzuwditmm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gupkqeyps.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gczwjvcit.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gvaxohxuh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/geggxawhm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwvhwxwq.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxbmnxqz.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyjnztvm.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhpjobcm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gtqgwbzbu.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtmddyfn.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gbolyrtlx.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/grpgdpfkw.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/ginluemxl.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdzoqrboc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gattohkmo.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gelpkajwb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrulanfl.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsnbdjtt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gcszvtnqg.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrzyrwvh.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthxxosme.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifvkklit.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gkiiymbsp.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gimbtyvds.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gwvnwjwqa.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqlarxwj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gvelbmpkd.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gxbmwfehw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkwhkrkp.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gjfgkwksq.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/goucuvxgd.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcpobvdb.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuqveueg.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gvsexdyqt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gramwccmo.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/getcgkjav.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagogzktt.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvdisokj.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfiefric.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govgkovul.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjphyysh.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxtmeehp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwvajahe.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/ggwkuufso.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gujpxzxhi.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhyktxrc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzweqagfz.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaheaezoq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gquwbjvyv.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/govbaqive.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzkbbjkz.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gznuesjzr.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gvlxdqmrf.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gqxwnuujp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgssvlam.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghealjcls.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtudworgv.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/ggjrbjode.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtemlcoet.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gqocyjcsv.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gmmbgamwo.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzbzzxdbu.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gbvzabkso.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/ghiwlslig.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghkudrgxd.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gnhiqyczw.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/guzjjzrah.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gojyunbzz.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhmmcifj.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrhgqwac.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gbpejuknw.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwkojuff.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyooyuhqr.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqthpnstm.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gehciitxi.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gucyfdjbs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gtyqqeouo.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/giqcnurvb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhviugpe.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gqcrwggio.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjvsgker.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjvzrezq.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfxvjmhj.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpobuyii.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcfvqwjw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gcmqdgygt.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gfyaneezd.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudtbabxt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwbgspfb.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgaqxfik.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxlimdey.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhmclcoo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgwehpkj.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gccfxvzuh.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqnwmrsa.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gvhatqlhf.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gqhibroxi.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gngwpgbjs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcktvilqg.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gdwgikuom.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gbhvdeqfv.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvfqfebj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gnzwmbcwi.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gwrsolktg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkrcqjtm.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/ggvbherjy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gevkxinxa.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gakukwjgq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/glajvskil.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwixmkme.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gpnvxlwll.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gjlifwbhq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gswmbrcai.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjstiqtwz.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnuoloup.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/ghvopsbjc.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmnpeomy.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gkxculskc.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/grdoquvsc.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gijtgsgch.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyivzahuv.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gyquftaaq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gyfnurkym.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqismudi.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gygieisff.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/grsrjnzlw.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrwrnikh.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gxqpesrbv.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjxftuds.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guevljoxg.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/glxvyorhb.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcjjfqoh.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrufmzwi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gayapoqja.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqlncptf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdtertwy.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/glupccnzy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqrrtjqc.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gpesklfym.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gimgrbgbl.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkvhbljz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gufexbogz.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gfzrgqtfs.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbdagufx.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqngolpkp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gushpwkuw.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gkyytmcyl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvribomm.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrrrjhaa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gjluubkkn.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gjutvuzmt.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gzxwknhsm.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gvtoiebxc.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gxjgankjq.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gzozwmovv.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcccyeozq.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gjztdnkml.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/ghosmyave.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gzdxrnpqq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqncfgedg.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/ghnlzzgar.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grkczguar.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gniochenz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwubzzxsz.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpubdvuc.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdwuzpcvc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/goefnndln.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gklmnnrrv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavxcsqku.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoltycpj.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gngihtmvw.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlgnybdc.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfmjgmgb.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gjedwlrny.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gteesybcn.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlbuaywo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gprohrhaq.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzvkshdn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjksnlwhl.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gsigzgwim.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/glpekdeiz.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gllbsbxcy.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuoiybug.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gkaqfgiwc.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gwniiqgzp.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdjjgpkz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gzwgvzowz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gpimqkajk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjzyfcia.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gbkrwmdic.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gqpibktgi.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqyphdfl.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqyhgbnr.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guetxxhdf.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/givxybvcp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gceegdryt.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/goxoorwbh.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkydfaphe.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gkkyceisc.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gghrtqthd.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfaofpma.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gafbcgqca.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gesdtgnly.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gthrchufk.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gdvdvhjru.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkutcaldk.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/grxctrtbb.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gwafrbots.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwhxzcew.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gouioitfc.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/ggwndddul.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gfnuctgwl.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gucufyfuo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gahjimxgx.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gujrsdsdb.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/ggzdqgwaa.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gvricexxi.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjidcwfn.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzaqaejei.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrdpnnct.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gxzrpfjuw.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/ggwhzoxyd.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gmbvohesa.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxyecaey.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizewzgby.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gxmrckvsf.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufykeuor.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkftzqkqn.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gbygksnod.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gnbtyswni.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gfosowgum.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjeieepn.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgnmuskg.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxcgpbrj.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnphyjtjs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gbgnsruql.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdnnsjqg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gukyfihso.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gaasnbogd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gdpddavwl.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gcijsglhy.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gogmxoqnl.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrsxjikl.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwgqfjfp.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyxxcfat.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyswbhotr.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtaioltf.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gojuhlcqq.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxqzndwj.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gycikfpqv.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gdiemdtyc.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwhpxpdr.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/glelqolwa.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfszzfic.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gjlaxhzjr.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamibyhqc.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnzdtoei.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafajbxnn.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gwjkpsnlk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/ggccfoteb.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/ggcpetsck.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/grunlliiw.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/govfeaaxb.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gxonatzgi.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gdhoookgt.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbymqhdv.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuxkkcaj.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/ggvtutuuw.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gravxfknr.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcphqkxj.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdfjqttb.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggatuxcen.sHtML


<!-- 参考信息 -->