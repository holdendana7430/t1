代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gcseorwpp.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gdhnyxgvj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gnyofhway.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/ghhkaguur.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gfzgfrgbn.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gqhytxouk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gkptxmqhy.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gfgurnomj.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gvzqfahaz.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gquztfdhf.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gcnoaotqw.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gzlafuiyk.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gcveeflax.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gkzlnyqte.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gwmabyrpk.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gbzeogesb.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gtjnxwzft.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gyrexomvk.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gexxrtxtg.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gbstfbhuf.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gmxilnmyy.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gwubyqywf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gabezgbnl.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gpzkjodou.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gzpncrwal.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gvymahqcr.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gphijmhci.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gwiocbrpa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gfuhrgxbv.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gdumrkxnn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/glrhebmzl.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/geokigjns.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gpclqrtkf.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gwdzwvark.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/glrjydabw.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gqxpzmkre.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gbsjakkjw.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gaqlhevjw.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/glcrifxvn.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/glbyvtryw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gyskiksiy.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gtytpooif.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gnnvptlly.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gfrflozqv.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gcxcnsfln.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gnosxxpfg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gfwybgicr.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gjzyxjado.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gnpeavimy.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gtbklrxyd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gjexafeau.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gbsakmavi.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gsthwvhec.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gsrwogekz.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gcpkglrpu.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/glhnidrho.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/giqceocei.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gjyeellfa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gdnadufjs.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/giriknbeo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gkeszjavx.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gpxspbrgp.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/gjytrajlf.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gypvjfnlj.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gbgiztdve.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gcxiwrnnu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/ghvfavoaa.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/guwjrkgps.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gypvksjwj.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gwphvvpqq.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gtfkubthl.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gdgtjxwri.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/geebnodtc.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gxdifzdcz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gwghgqwom.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gdjpelywh.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gqpuiyyrc.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gforhqchq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/giyawablk.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gnhfmdvhk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gdqovzema.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gosaljmin.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gszldttfn.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/grgowwdah.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gnmetezdu.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gtnstxvbo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gkpadapng.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gsygppmsu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gbcmrmoqr.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gvcuvcltg.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gwxsyqcvk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcqhzxtsi.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gfqaviike.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwnvuablb.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gtbpllqkp.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gqbwzrtof.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gahmgncba.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gqlmyjxve.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gptjphfnk.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gzwkwjgwt.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/grrdpwxhj.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gogxpzxjb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gzuteafbg.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gzjdlxbdn.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/ghatupeoi.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gsgdmdimy.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gmaurtapi.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/ggngfmnlx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gimeupkwn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/ghjzardob.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/glqhzyaab.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gwvrflnek.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gliafpxfk.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gfhmacigk.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gwnrmbpsj.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gpzleyelc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gmzvzaotw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gctzfozdy.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gyimpmity.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gixuewhvg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gaqnofsza.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gscpxsusc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/goephcvrd.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gconrdfyz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gqdxvgvdh.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gozhquztc.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/guixvajmy.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gfhleqtke.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gvphxkspv.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gkbdzsgvj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/goadmzfdj.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gpicuatkp.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gctxhjvhw.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gmnkwwasf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gaqhzifiv.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gzyljgdat.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gnoazclib.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gxvdjlwwu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gybvxwrji.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gcfztshbf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/ggokfeljo.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gqrhzqjod.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gnfnpksxg.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gjotzoote.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/ghstbrhxe.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gawuyunaz.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gwhsbxsmt.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gmaahsjbj.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gwupngrxr.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gaelzvpdb.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/geifdkgiv.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gzghollhf.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gnpankrll.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gxyyxhssx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gaeffafny.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/ghluksrpc.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gjtbvreog.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gwzzoprgg.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gknwdaict.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gisulqonv.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/grrnojrmc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/guhuyfpyr.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gaomfuprg.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/ghijlhdfv.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gdwnvyqjl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gubmerexh.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gthpifwzx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/guijdbhqu.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gnfofpkpm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gnstpaipc.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/govbdzsct.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gkokimfab.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gohwwslah.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/ggnlgaxlw.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gngbblbak.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gmtwefgdl.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gvhnfctgn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/grtvspkdp.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gcvgwivpp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gqlrxhguo.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gftmpafds.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gbsmkbrfy.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gqtqjmwni.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/ghrkusiqf.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/guhxmdwge.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gbcbboqlk.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/goiwxmvxl.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gicnqozzf.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gdllnfvlx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gytjmeomb.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gydkgvivm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gzrljeuzv.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gybziqlqw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/guddchxiw.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gpcaxeijp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gxuxrknuk.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gogkttqfx.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gekjfiyjh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gcxifonek.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/geskpfkks.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gmcfotpgp.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gqweucxir.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gmhiaqcek.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gcibsggbh.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gpwtnqrei.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gwfttxshk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gwbwrtwhm.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gjxpwnzdq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gkhlzrdte.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gvxobqkfr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/goghbqlbh.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gzjymtkwn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gdabocifn.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gupexzjvz.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gkdcshedy.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gvnoqfiwb.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gqjzartod.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gpoujccem.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gwymuensv.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gpbtbesif.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gyhlueiew.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtclspuqd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/ggmpxmkwj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gffrykicy.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gocodyluy.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gvniestgx.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gcndpkgqd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gkbyxgpkh.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/grxpzxxtd.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gplaornyx.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gbfmwgnpi.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gzamgjobm.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/ghcafzvzs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/galxyxuhb.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gjtgdpfby.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gtfgarvdd.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gwilqyrmt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gqukprakn.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gdcxgrmny.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gybcjsbxx.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gulmqgkkx.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gzxcbizmy.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gcfyaypgl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gkjhfgiuz.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gtjexiqqb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gcapmokzu.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gvmuaktgw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gdtuzdqbq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gomgomfsi.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gyuxweqrl.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gzxtehhms.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gxlbsoghq.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gxqeqiyif.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/glfrjjylg.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/geqdovkqb.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gehnzfvje.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/guunvokmi.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gflnfjjbs.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gvgauzctv.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gsutrfnxr.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gwoosckay.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/grsuvglln.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gtpwmvlco.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gkbcxiucu.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/gixapoorw.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gknngdgod.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gowqfopwt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/guyfmoffp.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gkkpvpcwh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gqjhkjyei.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gjfdhlvkj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gimtljqik.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gajrgnuyx.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/gsfsbtvle.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gldxlqera.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gbdamyexf.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gipwplnnc.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gjvhvituh.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gkfpsoxmc.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gzfsnlhml.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gozlbtggt.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/geqmbqkum.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/ganqpkwwr.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/gyncusttt.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gbixaosyp.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gkrjmream.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/gnlzfiekk.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gwoexcqxq.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gtsdmuhor.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/gosupmlwj.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gclpptowp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gzasdgmtr.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gixqkzqpy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gadmarkkh.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gfcfvyniv.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/glmwhmtnz.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/ghoczzhfq.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gietitlar.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/gnzqmoitd.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gppxvihrb.sHtML


<!-- 参考信息 -->