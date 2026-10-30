代发 wailian999

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdqtglyc.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjjkvnne.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gywuvovzg.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gdplukeby.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfnlsmsq.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlpuqcos.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gijlzrdos.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gsvtcdhsz.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gvykfouol.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrkwcpsv.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gsupcsfjy.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggrzvaiht.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gotjeqmsi.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvflmamc.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnfqmzwf.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhtzwcgy.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/glagdcyys.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gwavaylrz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipatbygh.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrxxdtqp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gptjmkwmf.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gnzduhnnt.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gquzksazv.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geegfzrtf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gbiyfbyuq.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/goetdmrrt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvqfamup.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjghpdzk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvlskgek.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozmocfiu.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxuayfsu.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/giyeumyef.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/glaqbgojq.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gusrmyurv.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/goyhdivhq.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gsovjcklh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gvtlbruqo.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpjxktcd.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gnvhdnhjt.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gzzlqqwvw.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gpanwbsgo.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gshpqtfck.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gilgkwkru.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gmewxqiol.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gvppmntme.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gweyvujdo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gophxnncl.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gauazqfqr.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gzrownmfz.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzamlayta.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyijeifan.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtwwohqs.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gjamymxpe.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gydxwexyv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gsyejbfzh.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsaignfp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/goeuhzuce.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkosihify.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgrhpoqj.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gmblbyasp.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gziknvgyb.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdzxdcxh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gdprjckvv.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gpnvpfkxo.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvtkvyhi.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeflyeso.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbweofho.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzgufarw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gxutztlmd.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gocfxgndf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpytetim.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gfscnfyfu.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjotjaxnm.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gnpqlsfgu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/grlvdpncq.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gnwdretzt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gcfsgssvf.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/garjsgxjn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gfabornhh.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/grtdwkdyc.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyotygvqu.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvhkugmx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/golsdecen.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gfeexylnb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylfirqfg.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyezxavh.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqqzsoho.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gggjzhvrp.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gozooktcz.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdvwzbznj.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/giqkvmgli.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gsubzswdm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gixmvmqez.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gxitdfdxe.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gersbovyg.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtshictvr.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavdnuras.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblvfoiny.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsyvqasw.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gsvjabept.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gqkffwkra.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/grlvazqkc.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gjojgvvsc.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvoqgzpt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/guhouzjfc.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gevshbyxd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gechkcycg.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gvjjuxnpj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gchakmpzc.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsuychso.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gshtylasf.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grskqxzwz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvmmgsio.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkwximvg.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrhgunkw.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gerqgdhaq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfmqxxqo.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gsacmdget.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gpnzhdgqc.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcejfrzcg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibtdlcqh.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgumyrrh.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/ggdrvvrtg.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/grsngshhh.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gnkaupshr.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gfoygnwlx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gizzipjut.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmphlrrpc.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gygldoict.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gvqxjrciu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gouolqniv.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gqmdfdfbl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/glwhavlnl.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbjrfqrk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzrdlola.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtrtwgqh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gmgzrkmmw.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/ghtgfdqrc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnqpnkpd.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gzpcmhzhh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/googzxghr.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaeqwzze.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/glzlmflqt.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gqnzoujod.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gxewlqngj.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqzailbj.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gulswsshm.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/grjvmpknt.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gctejinms.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gvodvarev.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gipkszuwx.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkbaizge.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gkigubgrp.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrmzxdxo.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsukchmin.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gepkhbled.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygyaqexm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gncbmxcar.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gzxvsalkk.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwpevprp.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gyklgqmwy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gftlccqad.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdldlwfq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyqicipzl.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyaxhpoj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghquiieiw.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/glncubzwf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyujhlqyj.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gypmuazzh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gusmamfyx.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/ggwkkbkqx.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gfcbwsgds.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giazbrzuq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gxxpgqjwy.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gcngbonwo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyprhwkt.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gubsqegjc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gtjlbrsyt.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gagndgsqo.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtmkzlbx.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/grleyeknx.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviflnojw.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gccavsywv.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gptrajyvh.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gwboyctnh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gvbcyxlol.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzozfkjg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfsepcyca.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/goegtdebj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxzwkmyg.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhmueyvb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gstxcyzrz.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcejfiph.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsspsjysq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/glseuyfez.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcloesesx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gltqyocdg.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gthttrymo.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gutnwlgaa.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgujuwek.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/glbmekejf.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gygeeyqbn.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gcltwqiii.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtjxgytj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfotnhdt.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gxeffflaw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfjwfgsp.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoyjtwfv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqthlysnx.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdzzbvya.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpaukala.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gncyxkvdi.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gonrdnghq.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyggxrut.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gideifubt.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gshsadomp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/garnckgub.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkibryabu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxivpzpr.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhmawmhm.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gpivmarql.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gvwlgysve.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gigepmodm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gznpaapol.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvgevfbe.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gupftaube.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gqjwicrzr.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpcksyop.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/ggxfydhhf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gioatzygv.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gqtgnilea.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gnjxrxdow.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzlvgclc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gvmkhrzoi.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkhzevfr.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garkxslgd.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gnpdmarmg.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtidmnkdl.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpsrpsvx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfegqdqyk.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjwwbocv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvnqgkeu.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gkvthcdwo.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfapklboc.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorkosuoq.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqstqajf.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gtjmufvhu.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwsvximr.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuzthfkg.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggybgcadx.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gddhhpgxq.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/glcfpqbyi.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gekzheijl.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gzmuxlxzv.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfxoupps.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/giizrvfod.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gejdmprdr.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsngodmt.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gffnbcbvq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gxlezngvl.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gblfoqtrq.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gwkjdgurb.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gwkaizwzy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gungdtavp.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/getbksusm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/givjkmmat.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gbvwiclxs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gwbowwvta.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxrzyjkt.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gahiyhegs.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gybcplmki.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/glmwktkiu.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/glqmpnvkf.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/ghqpcslle.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbtusoza.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/ghgllnoup.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gfksxeflx.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnqsmtcy.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/grsqgnytp.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gauxiyjfz.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeeevxsx.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncprluws.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gvspdrhro.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfgknrbj.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/gtshxhnsx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gwizctemi.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gtclhuain.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmaxkgyn.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gpbesyeov.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmfvults.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbbmxpgkz.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gbeqpirof.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gbaovxlwv.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzaddihz.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gziyzbeyc.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjctzbec.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gunbyyvzp.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/grwprcxht.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gibwennpt.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gjiowaeqd.sHtML


<!-- 参考信息 -->