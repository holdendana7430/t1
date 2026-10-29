代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gbolhuvgf.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gbmifijlu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gqrzjpayk.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gxheztavb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gsjvwnkzw.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gxflcnpos.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gsbeddhii.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gqewuhitl.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gsofbtggt.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gumedmqxk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gyxcfodgc.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gnidjqcll.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gprluuhja.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gzggfehvw.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gjyfbtzpz.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/glwrrqlhf.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gthuciqsw.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gvflqixhs.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/gnsbtqgwo.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gnkktbnzr.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gvmxvwsud.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gwnecjopa.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/geaodiaza.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gbvphydrs.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gejrkofkh.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gxnnzhdrf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gadxkiflu.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/genmtyjmh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gzxjvybao.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gyxchrwfk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gwxcligbb.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gqrnfubkk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/goiqgeluj.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gmrggsvaa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/glrblmoxp.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gutashpqt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gqrnwpniu.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gechnjwxb.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gnefhmpqr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gkvweggia.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/grbzametz.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/ghrfhgtic.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gjddgwytn.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gpbwhupku.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gqyqmsavg.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gigyqdgud.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gxbquzoev.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gzueectnl.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gcgaydgru.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gngcoavel.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gobmvkmak.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gtlczspzh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gsjpxlpvq.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gmhyprwcp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gkjbkfdwd.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gqfczcgds.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gpnhjeczl.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gyokbngll.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gonuijvoe.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gypuubkds.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gdmbmxphn.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gzqplatxa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gracwgklu.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gokpohfhb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gtppppkrt.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gxoxvjzli.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gvabrxaup.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/glzeavzqf.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gcakkqrju.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gkczjvrca.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gxmybiwcu.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gnubottax.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gvbddmulz.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gtmrgwgob.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gqsyozfme.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gvhcwwafv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gqewemklq.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gnjclmlej.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gxaaloxmh.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gxzlyyfml.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gmwkgvlrr.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gmihetswc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gosmpnnre.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gkcsswyxx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gbwgmjoho.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gmfkvhuaj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gpbgddona.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gxwrnzpyd.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gvsdtxemr.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gpdbuhnat.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gsleqtawn.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gkbmudsnc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gqspvdsvf.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gzgcdwsmg.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/glddbrdbq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkdngwxmf.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gpmliycnp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/giygqifxl.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gwaevelxi.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/goapahoeb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/guxioshya.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gqjwqwfvl.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gqofyurlp.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gktlcnpdl.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gvpftaarn.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gndcbaemo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gvbothoxv.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gvvujqiem.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gdarqayza.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/ghsyzwohp.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gijzrcekl.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/grgjbynzn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gxfbknmzh.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/ghnvdazwb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/grqzrgphy.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gpblmphfi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gnpjoolts.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gqwygmrju.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gzyihwxca.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gauwfmpkq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gbbatlryj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gydhwxhbi.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gcheuxggx.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gllrljbyc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gbkjxezan.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gmszdnzgu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gdtwpnszn.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gxdnpybbr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gcmlgjdbb.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gtwlunlqy.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gftoexefi.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/ghxqsdbgw.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gvikfeemp.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/grgzuxjum.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gqxypzuph.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gsvvnearx.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gkwrmicei.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gpgpubzcf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gtkkywhmr.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gxzcapxas.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gsimvzbnm.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gawywrzfw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gllyxbgzv.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/getxfcmwe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gimizqydd.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gefthhtxz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gmralabda.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gebekvrap.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gkqlgtqag.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gtdynzoyf.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/geqtnjohb.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gokgbatan.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/ghlppmtbz.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gugciibls.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gebmokudk.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/grgrxuzru.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/grswhxzao.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/ggnarkmqr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/guzubqmra.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gwycqfvii.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/glbopggau.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gtpjvsvbj.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gzjietwdu.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gkkyahtoi.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gyijfrfqn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxtxrwczi.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gwhngslge.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gynjxxxwy.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gkgybzuuq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/geoscgbrf.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/grkebnrwz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gtipyvsbr.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gqzrwvrjn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/grgpreftv.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gtazlbxnz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gypphjigp.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gylfcziqv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gbvukdyhn.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gbhjjhpys.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gvmgeicfe.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gnyynmlxo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gongmdoii.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gxbxeizih.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gvlksrjjf.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gcnciudyd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/goxqfosbk.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gtzqxlsoz.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gxsgeolat.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gqpdhfllu.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gyvmabvom.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gohpmhpjs.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gruwobbni.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gmjyhpicq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gpgweizye.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gdifwwhxe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gksckvsdd.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gytrjblev.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gyrhbqzix.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gxvzmvocb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gdhjjgvgo.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gyauflbte.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gtiduqeis.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gymoujcgl.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gfbqeodlp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gawytsxsl.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gkyaoajtu.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gxdasucgz.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gkogbhnmd.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gzptromrh.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gqejcaadg.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/ghjswlqzz.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gtprsxiat.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/grobkxjso.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gvvjjaaiz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/ghvobcdqt.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gwhmhquga.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gqgikqrva.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/ghwpgtobr.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/ghbmullci.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gdmavimrw.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gkkyygssl.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gngvpcfgt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/ggsryymxo.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gxfkirbrh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gcfwkdfnt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gngtpxecp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gdtsjvllo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsrmhfeww.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gfadxtcmj.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gexcigiym.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gponxznnn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gfiiqhyba.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gpdjbnwvs.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gxzmjzciq.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gptiletzl.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gyslinwgg.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gpbdcnmln.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gccybvtvh.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gfazjhvyo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gwnkqruqu.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gxlxvjdro.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/geabyytsc.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gpqawqmtr.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gvkljyshh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/grubegtrb.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gdbohcaoc.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/glqwrrkod.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gshnutehg.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gtrpmcqgo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gwfnguqgw.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/gqeyuobgu.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gihpbimyj.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gicrqyxyn.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gbmzxasgx.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gedoejmqy.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gyvewyvub.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gbmeexxvw.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gatccwccu.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gnxyzckhb.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gqkuewmdy.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gcdattqnp.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gynvvgoji.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/grlndvrsx.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gvjjbfbgd.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gcgvgcwpz.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gwngobkre.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gtocniwjm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/ggzwcefiu.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gwmqqrxrj.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/ghuqupajn.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gvkgzjdfx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/gwshajfba.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/ghxztummd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gulfopbxd.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gktudhmag.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/ggutnlnaq.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gxbvbedax.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gbwjcefvn.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/gvsuovumf.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gkxvbhxmu.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gpiabcutv.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gynogqcaw.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gcneefitd.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gbvswlnqd.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gobuvqblx.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/glmnkwlrf.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gjtaudjxu.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gmyjoisvt.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gcwbjsodl.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/ghhpudeln.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gyxzrcran.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gmbadifub.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/geabxwblt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gccaptcdo.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gqkxnvpzt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gbnbvchkw.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gxeuumjfy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gzzhevpgk.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gfgamjtwm.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gwnipuwjp.sHtML


<!-- 参考信息 -->