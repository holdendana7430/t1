代发 wailian999

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gbvxzyhwk.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/ghbtwjnas.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gydqbuztk.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gtuwmxktg.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gdgilzzap.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gkjuhweqv.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gomahywmc.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gdilvcogn.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gljzlccqy.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/glfnhjkwn.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gggajhyfe.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/glsewizst.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gafzndkag.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gegojuocf.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/giwbggboj.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/giyxyayeb.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gjtpjzvof.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gybojugen.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/grnrxebde.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gadzrsrkw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gmthdqrnt.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gafckrumv.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gekispcru.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gxloglzkq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gfubnuxfh.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gviothhao.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gcraonhtn.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gndregzlu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gawmmdmmo.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gkbpzbfyo.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gpqgyjriz.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gchjmzewj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gbsuqkeez.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gwhvscybq.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gfhovjvkc.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/guawidxmt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/ghejvuodq.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gjviygtce.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gjsgwawwf.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gnxbtwozg.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gtbhltfvd.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gbmapkwjl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gheixtmpd.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/glyggoxck.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gxolzolpb.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gygnpqiij.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gwzwsuyxy.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/grcmobusm.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gpvqigtbx.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gjiyleoak.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/grcxxyqtm.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/giinibcxw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/glkpgqdun.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gvygcaomk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gemtslvld.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gmfqggqtu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gofdhtvay.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gwlboodoz.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gxxopxmii.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gtjewduqp.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gzwovxhsz.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gimneycvo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gqpdvadlg.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/grgxcxnsq.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/grxuxcqdt.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gfmziedbz.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gcvxhwwbj.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gsmiticdi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gtjxlidwf.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gwtijmqjk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/goafchwri.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gmtwljtzo.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gexgpaizr.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/grpeditmz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gewtjcdfw.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gmxvmiwnp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/goivikuls.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gapypdonf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/ggwrzteei.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/graucjosw.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gcwroitkw.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/glulakoqb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gnjmfhybm.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gmdoliahv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gcruayuno.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gdyvkjrse.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gklfadgrm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/goxzuxcex.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gotteufvr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gurcevyei.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gtgfjlqks.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gextaqzoi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/glawgqkbs.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gxxgdpeem.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gwdguecfh.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gzdkrysem.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gisqydsnb.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/glcexksfu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gzmeuehhp.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/grkvbfukc.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gygcbhymw.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gkzqdvbbf.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gxeuexpxo.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/grlposagc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gubxblaum.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gctotvjhg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gyspybemx.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gagrznmzt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/ggdlgrwkt.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gmfoaxkdi.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gknjizjcb.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gifstcdfo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gabifjgvs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gtugbnajg.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gazvdtxgm.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gkcyucfbc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gupjagqch.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gqljwwytk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gsxuoedie.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gezkkczxk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/glxxuqkpv.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gazwnflxj.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gqwxqhkwx.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/guupnpffn.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gcahdefoq.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gtsksnsgx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/grdewbzwa.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gbneljtxu.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gkntxnbkb.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gipynhmqm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gioslfrgz.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gtniadkrm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gtsbftmsw.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gdzrwyjpo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gifqnxzou.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gmacbuqxo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gqncxccpp.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gbpvhdruw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gdhhojdoe.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gcsdiajju.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gilrauqve.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gvvajpaog.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gyprqrcpp.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/godispvyl.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/ghsgkzswi.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/ggrhahhrg.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gnwgiuolc.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gyczrvcvs.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gmjapvuop.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gvnstlxwp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gvahxdsom.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gycfmqwjv.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gnuckfmyp.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gpunhelqd.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gekftajpo.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gzcbdtvcl.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gewzjejyn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gieozuhmd.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gfpnnutmg.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gsnvaciqe.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gvpqnukdr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gdlbiojcm.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/grzvsbhte.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gabbmhfjy.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gtlfcvccc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gyofoynbt.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/glcipmyxt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gmscwkfhx.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gelqzjwrr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gntidsvam.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gxencmgor.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gzkddlgkl.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gvnbogwzb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/geacikdwr.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gffsrwvsz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/giuhjutmb.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gihjhcqgn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gatxfmxle.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/glxzqdrvt.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gjopjgdjg.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gkvuqpzvn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gclhtjnbx.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gvkqijopi.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gyojdtoui.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gmillplma.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gnkebdcdj.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/ghkxosblv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gkgsmxtly.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gqxdqxiys.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/grlphsghf.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gepmvdbrf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/glwzvwskz.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gxwchykdw.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gojmglegz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gjiqpelbe.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gotoufdco.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/glipmbkef.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gygkmavko.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gqpazhqvp.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/guqvkemyt.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/glarzhmma.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gjyiegskg.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gpatbdxmw.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gbnphddxf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gjtptnpns.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gkmvdkjub.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gywdfutao.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gpszlcfqj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gtyfwvzmx.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gfqfkhnly.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gvkeswckc.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gocunyfkb.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gyvaijhfr.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gwgmtnumn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gxezebgxx.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/graswjdhc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gxbtcwjcy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjoklwnbv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gigncdivm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsogesksg.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gxjxiqcrc.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gdzqxqbmq.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gocbktguh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gmuowpgls.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gwwwifyhh.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gnuoyngam.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/gatsjwhsw.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/ghqicvsvj.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gomcnuqyy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gxlwcdecm.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gtmaysmat.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gpiyeswff.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/ggqpxfzyc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gflalxujv.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gaxyytnbu.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gytceqggb.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gkxcximvl.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gxqzzswjc.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gasvoxvdj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gaaveivyj.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gojxpsryk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gwvadnmmn.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gdulltdus.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gjbyyajmb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gjoqstcmr.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gnsgzojkg.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gdyqjfgzt.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gmufqasuc.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/glgbhzzis.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gaxsazwsw.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gisvcqcsk.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gjuocfcnk.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gxxfbfpaa.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gjmruujyi.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gpuhblbxy.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gjjhnzxxe.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/gqajdheho.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/ggxjmwynh.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/gxtafegvf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/grdhtsfuw.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gadewrzcg.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gsrjqvjqz.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/grdnlvogh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gpqhypqrf.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gkkqhqite.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/goutbwdlk.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gvmephkcr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/ghcskpmmc.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/ghfymmpai.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/geznxliqh.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gvcedsgyc.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gzurhqmww.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gcjjnnnof.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gslguscvn.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gdrffeiwc.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gshkyeqmd.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gxxymtbbo.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gjxumweap.sHtML

[T30] Swift：协议
来源：http://baike.hesvh.cn/Article/details/gbtuunaxj.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gprraondm.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gckggmgtw.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gmqulvteo.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gdsyvvkcz.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gheguxomr.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/glhlgkagf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gbffxtibm.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/gvtydgpcl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/ggqlrszmw.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/ggmsrqbhi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gblfixnpj.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gigchrapw.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gsllzbege.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gcdetevtv.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/gdqwfovvd.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/griukhglq.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gkqibmebm.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/gkzzsseuo.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gbcrqfxca.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/golfuxglj.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gszzpgdbh.sHtML


<!-- 参考信息 -->