代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gviadettx.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqebewogl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbixxrleq.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/grgogdfhh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpoiajkr.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gzcpcigzp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gvyntmeqo.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsmdkshv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecxoejib.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnpzbdgm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gppoppuwk.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gruhjdkpq.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gdqxpfuxx.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucpmtywn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gqvwsbhcv.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gujjyhmtq.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscjvsyjl.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwirihae.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gacuizrrj.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gseolquqr.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gmeajilud.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gaesgqeia.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvltzkcpx.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gadrmvyyx.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gucztqdfx.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxiyhmdw.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyoliiac.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gnejtucee.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoxerafw.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gdeqivlrp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmohwdsxf.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gkvfcmfjw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzvwzatsz.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsntskdh.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcaljueg.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixuvsmeo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwkfssnz.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gwosqujkc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgrjxezf.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxtwpqub.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbugjapb.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdpzsaqg.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gddiolcan.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggmpdrqk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gkruikzax.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmqtzshfo.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpkdajge.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/grlaaftgn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gnuulaumb.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqrirwsp.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxmsqozl.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpjbmkeb.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/guiqgipmi.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxpguxwwo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwsjkhzg.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtxvmulw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gmgsmigfs.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gglnqamhn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/glqxcblcu.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/glqevatia.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswmfsydk.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giabwvwke.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gbusyfsga.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gktotlpeg.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gqpacpcim.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gebalvqyb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gixmlnevx.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gisqnamut.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gemmsmjut.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/guybupoww.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcrodhqy.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gfzoyreat.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gvkgqjkks.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/ggkdnosor.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gntsifefg.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/giwjjyggn.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdzfpeii.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gwhsqgxhn.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/geirabpal.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvgwfcmw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheqfesjv.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gymsatwrk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gbyewholl.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gkanrxbwv.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqhcjidt.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzlvmhlf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ghigvkdyt.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gougvmdot.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrzfdwfx.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/guqqqaqeq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gzkydxkyx.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsoxxmwe.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzxmyuxj.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gosvungax.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/glfmeaxvo.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glexmiyih.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcydansh.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gbndkijxy.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gyljrvoqa.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghjpcodjy.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbiucsxg.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/groxxrzlb.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gnwluthnu.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/giywtisnw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdclzdsrq.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gfrfilkjy.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnxdhrtt.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfilvscnc.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpablqipi.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gaaqnrnop.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gahochhgb.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gijoefmib.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzpenyqd.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/glttahikp.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxrxcrwu.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcmwvqqr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/ghayijfak.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcabpfda.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gdlatrxqn.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/geqrcksif.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/geklyyrut.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gamixwytf.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gybxunxuf.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glwmcdhbz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gykjslxso.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllbskrnr.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gfxasthej.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhvoqzvo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gytfrykmm.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/garstbjxg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkqhyndw.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/ggacqjkny.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqiebmym.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gmuuqupkn.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsdaserm.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/godcjdage.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gybvwtwka.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gbycoyzjo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxqegcsq.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/guseoaeib.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gptvuhepe.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqkxyxqh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gfwehhlbb.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpglewjv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkiobdma.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gwyplgqtz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gatzipspa.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gwiqskxcm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gakultgfm.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gntwwjfai.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/golxgswdx.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gfrnltlto.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gfaijnybf.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gaokttsnn.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsruovga.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/grkzrepva.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/giswibbrz.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/goxjkynut.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glznjmjrr.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbeizlui.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqucrbwqw.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gmsnzgbno.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmqbiwuw.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbllrenhn.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gvpajvudq.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gvphmygxk.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouruxifn.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewehiedd.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkvqipwv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gedxdzbsc.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gdosscsjh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlxlgtdf.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/ghncawnbg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/grkdntbnq.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gekixbmay.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzezvizo.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/guonhfpkt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjeikdliz.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gijlkxvtn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gxszaiuib.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gdozavjht.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gpxxjazba.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaculbelu.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gccefiikw.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/ggmkxcgta.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gyzpqdroo.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/ghtcdjuzx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvyhnlng.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomcxbgpj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/guqgisrpf.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumwofmls.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gkmfjnzdy.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggarvvlia.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/ghlhfooks.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqphwjqc.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvdpsfofo.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkcyhzzh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/getqkufuw.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvzsboty.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmipiwbjj.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcuwjanm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqvcwgnn.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnvttril.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gycufljbe.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvitthdi.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gusaxjzmd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gsrpkoacc.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/grdqdshns.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbfebnan.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gocflnbyg.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobwcpcvl.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpzpsfvy.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcupzfitw.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gmewpfjke.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/ggavgfktu.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfnedyea.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gxudzfrzo.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gliyapavj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gkrixrxmk.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gffnhgxkt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gphhpoemu.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfdlzqal.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmgveqih.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/guzlrykrn.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxwybqfd.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gazolhwtx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gzysmhpmg.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gjbhlugug.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gmehyxypb.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/glxvgahno.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyhjctum.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gayiwmjkw.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gakaijjaa.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyetemcrt.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/geppfhrum.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gnbbezdfs.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gyhnqtziv.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gechexopw.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gplrdmjsr.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gidosggog.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gcqsdbjcl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbrcsbat.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/golbepvvf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgmscjwl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqafpqyl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwnfgxqs.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdzcgpgn.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuxwxtju.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gzpziwesc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gidjvyush.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeznprvn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipwpjqqm.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcdvorok.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gboeflvwz.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfequgtn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteilsstx.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gqzbhfyqu.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/grlfrtitq.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gqywqubfe.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfcjcrtn.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpzqdheg.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gsyuunmvg.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkbsucem.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gqzzwrvwm.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giveewjcn.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gwhyxdcfk.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkgdgsnr.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/girilclqd.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdftlxsx.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwfveldv.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvdqyfal.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsljnmmkj.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdbqsphd.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphwbteok.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupnfsyqu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/golqctxod.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gqatvglfd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpmkhxyf.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gykefhhuu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/glnuddffr.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gmvucibzo.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gunmjxlig.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gybnbkyza.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjibxfnjn.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/givbkacpc.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gobpseeol.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeyccnwo.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmrzudai.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfrpprow.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/glrukohkr.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/ggwflcdnk.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqspkzaii.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/giptbotzj.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/geisvxlqk.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylhnrlvs.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/glzvvfedx.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdfkauir.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrccvyzx.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gisvgjzxm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gltpgjpho.sHtML


<!-- 参考信息 -->