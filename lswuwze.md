代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gljmpehtg.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gnzaslvgd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/grjqkgviw.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gqssghnhm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/gvbqfaaen.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gvsbrlrhh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gxgqzwnun.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/ggmnnqxqt.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gjwgorzxj.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gtlfcsgao.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gmpstzzid.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gzkgmuxuq.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gweofvxjk.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gufjyofuh.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/glunqsjal.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gtmlxrgmw.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gynzdmvuj.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gddpdsiwd.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gcjlwofyc.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gtdxgsdek.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gdzazymle.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gemqdamqd.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gxsmbwdkq.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/ggwyfreno.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gfiljyvwv.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gzruxjioj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/ggdgzcxam.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gnhqplfma.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gkzxviftr.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gcayzvfai.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gwuzxzteb.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gpszuvflp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gvnscmivt.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/giviqalmz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gqptwgbkg.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gijwpicey.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gpvktcnna.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gxpywdypq.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gzlyolmcd.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gikrlcyuh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gtprkdrea.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gnvnlivqv.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/glppnnfbc.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/ggyzrhvri.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/gzbebtgjf.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/grdlrzawa.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/grjzcrprt.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gmzmltlqi.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gczysdwlp.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gkruutvkw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gmwmqyfed.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gkfdwkgio.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gtawmzrxp.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gsiynfnlk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gqjocmwta.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gheonlqxd.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/ggulkooip.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gnnpyqwzd.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gernqtamo.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gtrndjylw.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gkzjalxkh.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gvfbxverw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gdfpsmslq.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gkzfbzcqp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/ginevkveg.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gpxvojiax.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gogpsbnrg.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gnyfakxok.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gsamwwwpj.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/giblnbzgn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gkccdmree.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gssjsxzlt.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gmugsphot.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gyxnusbut.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/guakplaxr.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gzgyxfrzx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/gocixwwvt.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gckpiduih.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gqznkuaux.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gmepktcie.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gcjiiguok.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gtcktvsws.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/grpxsrouk.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gxonqmlzl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gfsowbkty.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gcjyayosm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gaadskgyt.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gdmhuhrxo.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gdiunuapg.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gytsuhblc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gckblowlv.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gjewnrevw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/goplndmid.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gnxyjjqkc.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gmrhyguda.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfeqwdgtw.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gtdfuezef.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbbyeuqqn.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gkjafgjrz.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/grxsqutul.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gqqzhudxc.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gwtzfyjnw.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gfviipfdg.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gempnvnre.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gookqvqqv.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gphxbhgfh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gzttviqmf.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gyojrxflr.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gbtoyjxwu.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gvxkuuavy.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gwaegerbz.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/ggyjcdefm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gsgbctorw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gbbjscpyn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/gnomftrqj.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/ghnexfjnn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/garsrimxn.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gjurpprtj.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/glbeegvsw.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/giqawpllm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/goeerdbja.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gzecohpgh.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gdykjrpjm.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gvgqelxcy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gbxlbzdxu.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gqogpbncz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gkarfgieg.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gnsijtqoz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/ghkquefow.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gglrpsjuf.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gsaxksjhe.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gzuymycll.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gatiwygmc.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gjwumrkwe.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gyspnrciw.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gwfnldwzl.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gltfujyiw.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gmnqpamnj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/glpmvvihl.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gqntttron.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/grvrjhrmh.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/guwackelx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/giyfejvhh.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gwpyksaif.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gkbadaaxy.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/grxippqmm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/ghbnipvhc.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gkekxmhto.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gpjpganht.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gskscyuxi.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gxzmwahmk.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gzrvptuyj.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gujghwlxz.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gvamelhxx.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/grxyugsuc.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gcwsryboh.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gxnehuleu.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gckgevvxo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gmstypmva.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gsokrrzmg.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gbqhobfnt.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gmtqywazk.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gckpfvnvw.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/getznrjoj.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gnxzeawab.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gkklypehs.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gqlvbwskf.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gostgzgen.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gumyvzrqy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/grsslrkoe.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gzwzqzccw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/grpngddpf.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gjcvpgmso.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gktdhbsqt.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gxagbnxwo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gitqxjjhu.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gkqxxttke.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gpxkpozcb.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gxaxfcakf.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/ggwnepouq.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gjewajtsv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gnfcgcmmp.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gykosourk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gwbifanqb.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gfaqeatir.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gkvjdsado.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gqrmjvooc.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gdpdtbbgh.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gseralvnh.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gsehkujlx.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gizkvisee.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/ghmrjvldz.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gyazharyy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gruqakved.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gyqarsgpq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gabmppnbt.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gkqddrpsn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gitdxjqot.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gjyqkjicz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gqquhvmfr.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gcgjuvtaa.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gwouksrty.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/ghnaldxjc.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gabnkeyky.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gocwfakmz.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gdbditlur.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gaqunfgwu.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gecjavtkj.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/giuftznmy.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gisaqcumq.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gixtacwtj.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/girrohmzn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gtzzmgrjs.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gxgqpckbr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gohjqbujf.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gjcxmbykg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/ghyqcdqtk.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gczvzzaux.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/guzqditad.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/goivnlzza.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/ggihdgbwv.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gnynbypic.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gmsipdgfl.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/ggnfwtxpo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gbzggdwep.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gntlqwggy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gqtmgurpf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gekiaszxk.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/ggzxszqae.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/ghoxrulle.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gkuitfocu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gnhnyhpki.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gpuckdgxw.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/ggqmsjwce.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gfqdtzdos.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gouaxyavi.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gomkmqdhv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gqtyqjkmt.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/grpqxcuyx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/grysnmkre.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gonetelsi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/giebaegez.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gfnleikme.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gcizvxlum.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/guhpnteta.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gontqnfmn.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gcfzxoglh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gqmpqljaa.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gyokmipdr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gehjumfey.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gevmadywm.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gttokbrvu.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/grtoualkf.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gwdkrzveu.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gvglefjtw.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gsfmsqpsh.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gcathgwqo.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gxtwdlcjl.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gxzhiuxxx.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/genhoipcd.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gfasjlthk.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gtxawwusx.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gnutdrbue.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gcpegseje.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gucpvibbb.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gqvlulilc.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gsuyxkhgv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/gnpqtxwtf.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/ghmheoumz.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gafjpydzk.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gopprrzwk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gyfwdnkye.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/ghduzahpd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gwvcdrjch.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gxepjdmia.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/goprqzyiz.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gaxbidbiq.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gkdkwnoey.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gzivbuyqw.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gasfymdeb.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gkyddgthb.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/glksozoyd.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gdgvrurgz.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gyqbagpdo.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gjhzvkxiy.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gggtnyvbz.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gyuyiknzf.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gdvcszwvx.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gaczjfpze.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gspfozvso.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gyfpvoccc.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gisiiszjl.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gaaoyuito.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gdrwxdfsv.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gdidtxzvz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/gaaeltsaf.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/glqcrlzho.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gxnjuogyg.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gyodixfqu.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gpfeebzgq.sHtML


<!-- 参考信息 -->