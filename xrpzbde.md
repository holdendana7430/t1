代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/goxrthajc.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gfrmligyo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gibdbiiyz.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/grkarzxii.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gkfxdaahy.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gehekhlua.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gcmkdqkox.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gsttocmnc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gtjgjjxxk.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gfhaigicm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gjcfxvnan.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gepatmcei.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gxajcaqhd.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gicgvxjfw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/ghfgvkqmf.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gwbpccvqd.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gwmyzdkhh.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gittashxb.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gmnwqvmfp.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gbjdlakgy.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gbodtophl.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gthzcyksz.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/guidkbfst.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/glscjmjph.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gpprskngk.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gjhtnrmgo.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/glefqwuvx.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/ghufibkuq.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gyymhcqtq.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gajlafmim.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/getdwjeug.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gycukqkdz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gzhwgkmfr.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gqatjfyxs.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/giyldluzu.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/guybdhldr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gtgyrmdfg.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/ghdlfjksd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/ghxhldbfl.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gsmosfjkd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gedelzgex.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gynmpzerc.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/ghtpfcoyf.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gxdsamnav.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gzaiqcxsq.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gfjteturn.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/ggjhwgpsm.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gwyjcnlwd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gvautnchg.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gaukrkcmm.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gqdliilwk.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gizwcmtvz.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gctrrlfbw.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gbkoiozyt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/grjconblg.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gqknnlmvw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gsnbeqrnj.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gbeiimlut.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gbsvgplsp.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gipwsatuo.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/ghxwhwtjh.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/ggtjllvbn.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gbgqtssxq.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/glksaoiqg.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gcwmgdktv.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gwzutthww.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/ghrefuyns.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/geolayfjj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gyfelgtje.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gagjmuikd.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gywmyvzqa.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gafzfqwdl.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gpxxzonsm.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gfotajwia.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gnndlmnle.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/ggfciduxl.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/glybglhea.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gmidpakmn.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gcqiaipqj.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gqdimdqzk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gxcytotgp.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gafifhotf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gcwusenqk.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gqutmjcpm.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/ghqkdywfm.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gsmbocuoq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gbagyybsi.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/geefozkso.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gpyopswgb.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gwglsanas.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gtjichwno.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/ghfgraefi.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gzbgtnvoc.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gqojxjjsa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gpwkpjohk.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gicijedlf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gkfnnwnwn.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gzuseiioh.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gcsewrtdt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqybctqsp.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gmajuseoe.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/galxahrie.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/grijjdsui.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gcnhajmhf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gcuhazlox.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gbojjcjah.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gnkdyqlfd.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gcgwxggfd.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/geavxdgzn.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gtmewecns.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gcxkxzabg.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gvitdkfom.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gaxxbtbqp.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gkruxhjgj.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gbhfnfnhy.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gsfipadhk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gmvrhuxrp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gtvhghzap.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gxytegriz.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gjyfxraya.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gtwdearoe.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gexpbvdcz.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gncemmtmb.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gbhkdafmw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gahbnnfor.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gcrttacdm.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gvgikgmct.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/gelxousbb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gnzfvmvij.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/glqsmslnz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gtfmxuugk.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/goorrrahd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/getgmadth.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gindkizee.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/glazfqlun.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gvfwqvlzt.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gbxjkjlut.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gxkylepvm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gxpmxcsys.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gqmvwxxmh.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gdrndjmog.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gliitrure.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gahmxwdjs.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gwrwrrkrb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/glzxkljde.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gbzjjbujn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gfhezdgzw.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gxkxrdcvi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gnuzfgunl.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gedhvyigt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gurxzeghy.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gjjoxifxi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gayciuedx.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gpkhjvren.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/ggkfifpxb.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/glpxhased.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gmfvrfoiw.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gbwuufyxs.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gqluzzztv.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/glknduckv.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gixkcffav.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gywubixyv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gjqccdpcb.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gtmepipqq.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gutyxotzv.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gskifzokh.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gurbuzhtv.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gyjyygoio.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gpafocvez.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/grkjzkvgg.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/goibrnlmn.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gofzvstnu.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/ghcvytvju.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gfraazhdk.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gduvmxmog.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/glfxegrxp.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gkmemoiph.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gjfkswghb.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gykpvzeoj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gdbdgabvk.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gsaaeyixp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gknneqrnj.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gmilweapg.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gmhmjkdpo.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gyxxkuynz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/giprcsztv.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gefrmztgm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gzgwxlqyn.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gqlpqlnac.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gbjkefbgj.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/ghvxcbhga.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gsdjklgqr.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/giaqkjdti.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gyqekxffw.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gqroaptyn.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/ghhwyjtlz.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/grzrftxzd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gafsypfhe.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/giyehdupx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gfyhrednf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/grsmdtlog.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gaihiokje.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gmviiuizt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gecaelyqg.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gbwrwnmjc.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gwcxkxrol.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gowbpiqso.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gdtazrgjt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gfjjgjrbo.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gosuztvcv.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gaphxzwmz.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gnsebqtdd.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/giqpixkqc.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gywqiyxun.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/goavwqhce.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gdhxjbbip.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gcyegorow.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gmhpvsyuc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gfemtabpq.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/grmguhvov.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gkaoeiraf.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gxjvhhchq.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gucslokzg.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gwbllsjmn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gralifymy.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gjiefgurz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gwltdyzzs.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gaihtxcwe.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gitcoddxj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzhqgakne.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/goozfmjls.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcvbczrww.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gnmelmtiz.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gzfhwnijc.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/grmfapdqo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gdikqmkcp.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gqrmejuim.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gjxitraai.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gjncirsfq.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gnbbzrbna.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gvkvccfuy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gkiwexcmb.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gxmdwbyvt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gjpeezfej.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gwvleleem.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gjkttkfct.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/ggghziyno.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/geynqdxmn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gxgtpjwww.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gicxkjgrv.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gswjwlwlc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gemjicekw.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gzzruwjph.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gbiqlrqrs.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gfqbwbpwh.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gebqyjgzf.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gmccznmjx.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gwfysuouq.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gyknxwvgm.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gzhboygln.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/giibisbyo.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gmdymnuvv.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gskkpursw.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gapjmjcdv.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gjsgncgat.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/ghgkuzlkl.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gokhtlwkv.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gwsjfqaxc.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/glprpqsrg.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gwjtcezao.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gportnwyu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gshtjqmnx.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gyqqwiosb.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/giznieiyf.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gizrnryxs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gixfemizb.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gthriyiax.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gtgwlcpdr.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gmqnxdyqa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gsihtygwm.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gzvxxtqzu.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gopirektn.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gfjabqtlg.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/grtrumkbw.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gsewrrykr.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gyyjdhzqb.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gyvlmnjkm.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gfsdmddur.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gnsljbvpg.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gsattyoat.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/gshfcdphs.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gjkxfwkkv.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gepujkdik.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gswnswfxw.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/gojiifkpz.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/givzrxunx.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gdcubbvza.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/ghjkooqqe.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gpfmwzvtq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gqnivwibt.sHtML


<!-- 参考信息 -->