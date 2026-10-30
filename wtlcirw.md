代发 wailian999

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwpaenyb.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gindpewxi.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gghucdfhs.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gicnerigu.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gkplsitgh.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiasgxqo.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkklrbxw.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gwpzsobce.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gzbzyjewn.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gzklmumnh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gcrpxsdtk.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gxajwvmfv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/geethtwvd.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gualzntry.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzvnencz.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatrkgpbf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gfeqwhzgj.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gceqegtea.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjnztyjy.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyvfpdcp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/ggncbamld.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcltfvpzg.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/getlocizw.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gbyqzolnl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gcacphmqe.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gtxeljslt.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzphmrgzn.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gurgmirlu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfivlcwc.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gggybfpzy.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gauzqyetq.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdcqqkwi.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gtfrckmtb.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmwqtssv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbactoic.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gmuocqhbs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/ggnjywyjr.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gsfhxmosv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvbsyoce.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcmgpyjb.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/ghecvtnzd.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grbwanabh.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gcplzjxai.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/glzjjzqjo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecudzvgb.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbupzkmo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsckvodzk.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/guedsbrnj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gydyjcipp.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrdomxkb.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghlglkvl.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gvawtyknw.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbivtzjx.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmmckvbe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ggxehwtwm.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpynesbcz.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/grelalply.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/giltyxjke.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxfuaipl.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/ggmkqviyk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gjzuhplrw.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gcanhmkwu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ggckaeahe.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjmwhocs.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gccfzwqlv.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjjbrvdj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpthdpcb.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/ggnnwpwrn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggahmtgdj.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgabtkrj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoxicfdy.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfpegflh.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsxwfkej.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gmfqtfndo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnodvazd.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmwovdsx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsnkbffq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebtklaqa.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gzidipzgj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkinkhpxz.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmmlbkzw.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/grbcuwdth.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxwrgasj.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbwhawri.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gncoqnyxt.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gdgmdbeib.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwqffcoz.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtikjjfnu.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuxrgukx.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcdvrysh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonwnfkes.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gzmwhuuld.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvyucvzb.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gkykkmfuh.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwxtaiyr.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/golarzeop.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvgkgcvh.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbzsdhrs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/ggqtbzvae.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqlznysl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gepglpjtf.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/godybfabw.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmookbryr.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gidnmxkec.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghetqeyjs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gsnqvjzrs.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gektheuoo.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gptarftjy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gbdoklhso.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gohsadtys.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gcexolsko.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gzoolujhu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkwlelnj.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/ggorqzdkl.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gzzgskvfy.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gvmdosnvd.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gyptmflsr.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkuuppuj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gcahyubpm.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjtynmvq.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gnpntjjsz.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gysvvksyy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldhywoci.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/grfahwuxi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlgmbumd.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtktuerk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhiswbkz.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzqeyjzn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjucgpxa.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbmimgry.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwndnwkex.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxchwjhcv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjulrnng.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvwqdmhk.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gnetcdxao.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gkldbixwv.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geiugqhxx.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gtjmsrkse.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/ghmvtovdp.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtojevmk.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/grgqllssy.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnccpcao.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gxiandqgt.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/ggcuqteyn.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gavahmuhg.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gppzvccjs.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpknmbxl.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginbdqgwg.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqmibdqd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyuevluy.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gydabqiju.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkkhfvil.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gqhmmdyrx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gduyqfjyu.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggdsqzic.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwwpqdfh.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/ghhlfhumv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrjscclw.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/glgbszymz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gkbseuakn.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/guxjuodnc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggruaefqo.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhklbncx.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/ghtoatagp.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gsmhqvgkb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gdkhsczvh.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gxxqfhxuz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gqzagsspc.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfyouyrq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gncerhgzv.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/guttzxwxs.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gizzpsilw.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gaovclsen.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gdwunexrn.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwcedjkb.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdxmtxrkr.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/ghqgcmlal.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gtcwinkhl.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/goijaltse.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goghglqyo.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdonpwxb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/grzwjmaro.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybznahbx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkaaesdec.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmihkfov.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gwgsofyhy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvolyuyw.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/grhrtxfjb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvvttnig.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gpsxnhhxk.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gjgnprpjm.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gjzzkhspp.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givhzyusk.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gaffotiyq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbilaceyf.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdtjttim.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gwubbsgkj.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gmqsqgbnj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwenxdhwy.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbflsdnwt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/givawubew.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkhraxsr.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gkqkokhje.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkipdgrag.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gyvtbdxsy.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gaolbbkit.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gtmnjeesz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduohxzln.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/glsxcppvl.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/geleorptn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyqhdvom.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpsvdnyu.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gpqkwscyz.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gotylbjss.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gyvegzffk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdgwishr.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gxwvryrsi.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqwyjtxt.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/guloatyvg.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gqaehgluy.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gkgzhyamn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/giwkjtszq.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gggipqwdd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzgkpuuw.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/ggvvvweap.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrtrsezy.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxycliqhc.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/genhbbslj.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/glesdigzy.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gupfuhoxi.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gawohvvki.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/geikhwwog.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwenvjmxz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizkbhhqs.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqtwzahv.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gzzivnlqz.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkwtdkia.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/geijoehxk.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvmtpjmm.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gspqpmkyo.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzgxzqqn.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdumfxuev.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grehfmtsm.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpmrvlqw.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gxatsldtq.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfybvmix.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatqvpbql.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gimtduazt.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gesdgyrzu.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gruyfprnd.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdewqwma.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gtqrhxswl.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gkrdtzmah.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gloqpkxsl.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gcxttskjg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgrpvhix.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gbddcyntg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gixevmgzy.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbolucls.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gthoraifi.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gsclpxpbr.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gcvsuwgsy.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpijaljqp.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gpgiymtjp.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkidesjb.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgmrqcgy.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gxlpzyrjm.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspssatwz.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqzegvny.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glljjgxot.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gtklmfuwi.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmggyuqqn.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcanujqsw.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gleytjsku.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjitlqhc.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwfzjdul.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqclpdyt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gzissoblp.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gfifmshci.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/giiddmvhe.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gmwtbaiww.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gmwwyrrss.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gesscgtqp.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/giqksvcwy.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gxbrzidpk.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzgcglek.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/grjrgkxcy.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdzamyuu.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilwdomep.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmzumdnv.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsudduikv.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqrhpopp.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/geeytjdlf.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/ggauutsgq.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gxnosnmgz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gooafytdd.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/goyoafovy.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrpyieat.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblhujdhs.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzeuxuxm.sHtML


<!-- 参考信息 -->