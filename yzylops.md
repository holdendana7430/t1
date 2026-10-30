代发 wailian999

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gjcfxibsf.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gexgcskzw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gyxtgzync.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/guopadxpw.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gacwlymve.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gqfipdodj.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/guqhjbjux.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/grxdrrbep.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gfihitkjz.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gdhwjzrrr.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gdhmiicsa.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gojlpfxki.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/ghdauqqdt.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/ggacqshuz.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/givfnjwdn.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gxkwywvuo.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gdgizsonm.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gobirglbm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/ggwchuedm.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gdzlrndhf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/goysiqage.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/ggkvrwoqi.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gynzonpfj.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gisdthmdj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gebxxkvqw.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/ghulmvrpn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/ginnzonao.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/geqhbuyzt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gmkdlwlvg.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gxdyexovv.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gvlhltpru.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gkgbjkqgr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/ggrkgevoc.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/ggahmqnyu.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gdkejiock.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gmokpqjje.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/goglhvaxz.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gipjmxutf.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gzsjttkcy.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gylbrqmat.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gruyubdew.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gltubacgb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gsluhwlnq.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/ggwwdxtty.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gwukzuxfh.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gkifzfpiy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gnnkdzrjg.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/grhoptgzl.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/giuhxkocb.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gmssrethx.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gjbhyebgb.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gsrlbmxlk.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gcsvcgpmz.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gcdrtztaw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gobmecujb.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gkbuvluwg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/geaybwhjr.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gfnorhutx.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gncxymezx.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gaxpmblep.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/ggwnrqidd.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/ghiitojwa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gkobxnirg.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gjawtgzhe.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gmnqstrrb.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/glsbilwiv.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gnegxdmye.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gdunmlqbx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gyaamexvy.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gvxrxligd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gbqpqnsmh.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gbghgidbp.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gkbtgpjah.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gifeqrxet.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gwmbkqidz.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gsrdihzzu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gdobeejto.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gkqgqlfir.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/grrycqozk.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gchnnjwxg.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/guwnhnpdc.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/grgdvrged.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gpphscppw.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/ggzndujax.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gmnrdnyut.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/ghhwiktml.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gqpefoqff.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggubccdaa.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/galkszwbi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdwempuqz.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gofdtpnuf.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gobjggkdj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gleksbrkj.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gzebhtfzi.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gsrdgqmpq.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gtgmareks.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gyvyjfkoz.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gwcpbfriy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gybhwlrha.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gcypwfoed.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gfuacaybg.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gsiarzmiz.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gcsisvarj.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gatqvoqoi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gdvolpgrt.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gqmjkeujy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gxqihfkhs.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gfwqffubx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gldwlcxqr.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gqwnmdysj.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gdrjvgaau.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gnbvmytem.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gyxnsaqpd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gaaygdyke.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gqflkxitx.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gdmkcynru.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gsahaioqm.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gupfwevhm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/ggnbnobin.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gcttqsykj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gedgcpgkh.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gietnuekr.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gjtlwhyaw.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gvoqrtozc.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gvcrqvveh.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gcrbwctwj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/ghhldrkxg.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gxesexhhr.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gflbapvqw.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gtfrizbcc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gwedkipmo.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gjutbrkme.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gspggxoet.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/goziaaqdv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gjxmtzwvd.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/ghnpunljl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gzjvrbrej.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/ggwvhqner.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/grbvqpjes.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/ghwhkjtmg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gsihcfwkc.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/guvnhddqm.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gpzwufkrc.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/grdewtlof.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gsgxqazxi.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gjdpyztga.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gbdofmsuf.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/ghdrotutd.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gwmjiglzt.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gpmemjscc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gmjekgufo.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gknrkemvr.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gdhckckms.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gefkquuyt.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gvnvnxegu.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gjphkxfjd.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gvmkuvzsc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gowocexuh.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/ggxwobtji.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gssxicjti.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gajurzbvb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gtxwpzxlx.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/ghkhgjsnu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gwurhwqqj.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gaxyktdxr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gilgecbyy.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gvcfbmgzk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gjqlnsodp.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gudgxmojc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/glpmnkpdc.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gjchoxcik.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gruzzbhja.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gcpyuopfp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gtrwdwxhb.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gktpkjwrt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gnmhzlxko.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/glzwiiitv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gtdmhyyqd.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gxtttbact.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gyxbgvuir.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gopujusva.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gmawaczgl.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gllfrqgwo.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gzzgbgues.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gkoffygrc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gprhyijej.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gstrqwouv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gkzhbjwfk.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gdgshcxfw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gdfctfgah.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gkcciprwr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gijapkqzc.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/glpygqqay.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gatjruesq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gvpoesvil.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gkfojomec.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gfgywgnxp.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/grgegmono.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gnarlqguj.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gtotplvqe.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gzntmjxcu.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gjfptnjvo.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/givxvbkog.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gifjfdjvg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gstmwhwlx.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gdaosbpfb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gwrmxcgyd.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gcowkpqsy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/grubeqedj.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/glyecjlhh.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gyebcfbxo.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gtoipkaal.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gkyeqtbsy.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gkmokyxyp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/geklchskh.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gtbmouuvz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gpjmfcpzh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggnztmtzb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gxfqekela.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvowmahbq.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gtdsjefst.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gttjahczs.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gxidklhmi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/grmhsjmoj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gmtyuikba.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gslmwdzva.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gyugdzhpv.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gefmgkvji.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gjgjzhobc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/guxfvdlak.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gftqogimy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/gmuhklhrb.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/grjfjjioc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gnfmdiarm.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/griontzba.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gfnsryjqp.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gbzrmcxrs.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gsiocmovr.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gccgmzilr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/ghstbtpcw.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gqpmforhx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gacbzgvsj.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gfphghcmk.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/glgryhapv.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gfiwcyggp.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/goxpzhjpv.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gdlzrsxyy.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/grrcwfaln.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gozvxsezo.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gywpndzgt.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gpoxbhqrl.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gwxpajefn.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gdzgmkjby.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gglqrntrk.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gdezywdxc.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gohmdozzc.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gndkxkvwv.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gdzvstvqq.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gccoegdbl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gujrowiha.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gqwaoicqq.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gezvvalma.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gfkxghzzy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gskqzugpx.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gbfozyakt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gcwsuxkhx.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gbvdpsand.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gthsnfukf.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gbalzpjer.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/geglufrfq.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/glkaxdjte.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gjqklsbln.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/godxcopox.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gosendeqv.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gjnipesmy.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gwpallmqf.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/grgnsieru.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/gwskscjvk.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/ggzcntman.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/glqprxxwp.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gdqtgmwap.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gqlmidgun.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gtahjjxms.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gbnppiyfu.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gzjbacpkg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gdokyretz.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gvaghqbjx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/giwmakxmp.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gxrtvjydu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gwmjvrzfv.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gccnhkgbd.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gbwvefext.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gpirfwtnz.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gxuzfvbxj.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gqgjqolyr.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gaesnvhwx.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gcvsaqtnv.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gyygdjnnv.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/ghyyshwjr.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/gmjdxobdk.sHtML


<!-- 参考信息 -->