代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/ghpfbbgdt.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gcaattsud.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gbgyjbagn.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gnnoblacr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/ghwexhjzm.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gldaerhuv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gwvlzcowk.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gcgljifws.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gohfyedlz.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gukvqimbc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gyfwbiief.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gutptkghq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gzzpmogvi.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gbevtgget.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gmiwfqkng.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gzrkplsvu.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gmkpemtdf.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gqkogmlet.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/ghrytgjze.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/ghycgwzvd.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gxkleekql.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gkxuzecae.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/geteqesow.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gcpxiovsi.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gbjiotkmh.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/gtmazpupi.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gkbfebsep.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gaycmtain.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gpeukkdku.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gdugcnuwf.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gtivkyocy.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gwwhipafs.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gwpmhdrgo.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gungpixtq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gmepcodwy.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/grhsmliay.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gpuqucdsa.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gvwcvbhta.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/grccfisfc.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gpgvrypzy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gdoeojyhf.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gjbpmnljd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gxmffsoop.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gzphuawmf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gauzezpeo.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/grthicgnr.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gspcwpmnj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gyvcisweg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gajglornp.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gmswqnfuy.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gyjmsjudf.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gpkjzxlqs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gbrfmvqyw.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gghaitpnz.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gnxqcrgpx.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gvjwedbkb.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gbkfsakdl.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gqmagkhuy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/glxypomlz.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/ghlfaqefh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gzpjhpeod.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gyeegrxbi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gvajvwjhy.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gknljzdcy.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gasifszja.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/guuqumead.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/grfhpcolh.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gaabljgwr.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/godoyvhpv.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gpkfrprln.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gmmispzrl.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gxxjxwtdz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gzjiwiikn.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gxnpgpcvb.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gcgnzhpps.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gaudoxzhh.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gvzypqbew.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/glmdtuthf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gsbkarnqe.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gcpxutdrl.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gpshwxbgf.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gyxaxhaig.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gusjbvmcr.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gsxjhwshi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gnuekxvhm.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/ggzttmurw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gwwehaqug.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gylxxhdux.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gjidccqya.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gsxkxzyen.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/glsshguas.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/grfzdunba.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gvohgjjlk.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gqkrsosva.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/ghwfnyvaq.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/ghbieuifr.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gfqokvlrv.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gjytonkqw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gfbuvtcgo.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gdaqedods.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gxzpqqgbg.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gprdasbpv.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gimwgbffc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcxyusqlj.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/glqvsjrjc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbnfinqwr.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gfhtmhgsz.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gbtkdghvv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gontssgmb.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gqubnkbmb.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gdkveqkcz.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gshjbltjd.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gsrnkllqd.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gdlegaluh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gpvxnothe.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gnbebrdem.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gfylozqzj.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/glqqtxrjn.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gfkfzpkmg.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gzmxkuiyw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gsagbohlg.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gacwwrids.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gkfweulup.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gjnytpded.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gmacxmmxd.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gnibkzsvx.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gjbfrxsxu.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gxqzmgnci.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gjqqpptei.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gvbzjuksl.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gcirhioos.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gpihicife.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gnoluszgg.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gudkmttse.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gkxloafzq.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gikbewqym.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gvzliljnb.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/griyojulf.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gcbjncolt.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/ghudeqrjc.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/ghsbhwvod.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gqnsqilkk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gtwhseulr.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gjywhxzzb.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gbftgdeqt.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gootjfkpd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/glbtxgrpq.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gwsofdlfx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/ggxpzpisw.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gxevcpuse.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gvsnppetx.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gzufrlich.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/ghmyafysr.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gswwtlmsq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gwxqrfifq.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gkbbqomhs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gpqgqfbvk.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gxqclrfua.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gcpmksxvj.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gmgqkrucs.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gjmwajusn.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gtrzinwkc.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gubujbzfb.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gfbvwtcge.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/ghawfckxs.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gsevrrfrr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/ghslwkfhp.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/grcoxvjps.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gjiiuayiq.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gzgjhtgpp.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/grghfeiad.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gvuattfxx.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gmutxfebr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gogxadusy.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gaeacrzqv.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gxjwcmoet.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gzafcagpu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/grswldmdq.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gztxpbkhy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gyfreldgs.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/ghrupjfug.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gfsxeuopo.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gunvkvlhv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gmkibdces.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gmkslorij.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gcnknwsik.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gjbqsxtiy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gnwxgslge.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gmxwtoaav.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gnqehtufn.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/ggobopmep.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/ggrcuqhgu.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/guwppiurf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gofpylbsl.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/geiwbqzjj.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gibdyfttq.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gbxxryown.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gmditcevr.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gulpkheyo.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gactdhhah.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gshmecohf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gqawotpbk.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gdyldbipu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gggqonlzh.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gkvwwucoi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/ghvdrosef.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gokrtnfri.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gqrcwqusn.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gzoohblut.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gjjapfuib.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gcpsczrof.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gvvzwholr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gznfhviwl.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gmmeknryj.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gttkczwsi.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gwkrfywcm.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/glmrphyuc.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gcuiwphvg.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gqjwprwom.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gtwzyvqiz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gbywmassg.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gpmucmbrf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gjhoidkip.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gmpbgmevk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/grsivfols.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gyiplffir.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gbopholry.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gfsdozdxx.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/graveyccx.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gctrdodrm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gthifaubl.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gxmqnsxgc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gghxpvtkh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzbiodihe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/ggvbiedod.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gesububjw.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gbpyrdkzc.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gnrtbucrf.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/guhwixwlu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gelhtdacy.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gycjulkrc.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gkxvscsxr.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gepvyvrxx.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gwsxkpidi.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gyraixicf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gjxqnxwfu.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gqflonsro.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gqzuvdwma.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gssvifmvz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gifbzoash.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gdiscuktb.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gggzlvzkg.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gpzudpksz.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gihfvsfqi.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/glyzhdzzt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/galohatue.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gsmjokoli.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gjmhbgrpv.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gdeejrjpz.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gasgsohov.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gnbpnpimf.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/grgjhbwxn.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gtkdgsfmj.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gccxllhlv.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/glwembudt.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/ghquaakxy.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gtaosgsed.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gsrppblzc.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/gftcypxyn.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gymrapeaf.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gcmgkhwqg.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gclgglzbo.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/gtqchtrgn.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gwjxnwykc.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gutogjpmt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/gogkdmjkx.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gurosobtg.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gjdemuasz.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gncoxneop.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gxyrszmdk.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gghqrowao.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gpzuhydbg.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/geulzfesx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gtezuylzy.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/gsigvvzah.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/goifiseaa.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/ggehxcfjd.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gbmadxulg.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/grqpljwgd.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gwmhhsmli.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gdnghachx.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gwdnnirek.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gdvrfrvme.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gyhynynqo.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gctwuhmsm.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gcexcitnf.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gpdbxlyei.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gcgjnpbhm.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/garjmlepq.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/ghilsnjxh.sHtML


<!-- 参考信息 -->