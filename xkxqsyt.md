代发 wailian999

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gmdsqiloo.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gdlclpkeu.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/grdqorjhg.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gtcrqunqc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gzuoolhdd.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gagshhvyl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gszuentzo.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gkjmnbqgz.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gywbyzgcg.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/grgpnkifz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/geeouixpf.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gilmmbscl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gjswoztkb.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gxsdhykdk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gswriwjmj.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gpzcynkuh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gzrxyyujo.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gquqiqjeb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gccenilyv.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gejkhnact.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/greukekxc.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gsavibbzn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/goxklnekc.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/getnvtqsp.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/grdmqrcyp.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/ghufdmhwg.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gzbdjtrip.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/ghhiboxaj.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gtgutoevo.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gmscspzvc.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gjyxooayh.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gpvbjutlb.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gxovawlwo.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gfpwmyfuk.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gsmcbmiqj.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/glqyirnab.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/giadcnqhj.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gtmcrozuk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/glxapyqxx.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gxgxwlown.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gewfhsjbp.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gufgkkfbd.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gpuizzzdy.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gsknzycbx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gjnrfjnvz.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gdoqzlpht.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gqcrtwjpd.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gkmmcaund.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gejakmfri.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gxfhdkkxi.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gvwerchbq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gqybrjyaz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gwerdzvcu.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gpsmvfgol.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gvhfmmugv.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gbjtgapah.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/ghmtyjuwt.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gyrkmvuup.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gnexzsbrv.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gfsqjfaph.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gdcudvmyb.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gmucqfvit.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gpzdnwblo.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gmeokzxns.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gcdmftodk.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gqvgpthwb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/grvhjoudg.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gigwcadid.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gkpneshlp.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gqfwftabp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/greqbdsjr.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gdtuegvwv.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gcgnwseqh.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gqkjnecca.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gdrrzmlvg.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gfggpdbum.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gxprejdyy.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gvfatpfta.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gkacmdwki.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gcaitfqmc.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gaqwmohjw.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gahhhmomb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gwldplqqz.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gobpdsvbh.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gcwkvktjt.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gcdukedsp.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gqbigwkoa.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gflnpjyby.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gzzttetnh.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gyfslnage.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gfmvksutw.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gtbvqnnog.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gusisemwj.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gjibhijlm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/glceulqzg.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/ghyjvnpft.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/guzmdvpzt.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gmdvqqbgk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gmpxxdmha.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gmngtahgp.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gaplpoibl.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gtvtvqkax.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gzvqnovdk.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/ggsqrccjj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gwmwpymdm.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/glwaskuht.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gbsmzhobm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzbqxdsyq.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gpdvvflvu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gliqpbtli.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gaouzvbjg.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gdgnzkyyx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbavrkdhr.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gfomhyznm.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gpavtbdzj.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gpnnwyumd.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gsldfbgpc.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gqyfumpcz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gwulwpzqr.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gdofadqge.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gpzffiwoj.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gulbktbxj.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gyudgbayw.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/ghhymajhc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/glijjkgnr.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gxsrtesyk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gawzmcacd.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/ggyocatwo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/ggsgzqsxp.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gidbwfdnc.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gmmdeofqk.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gecqpmine.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/grxpauqze.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/guuqndsup.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gbwwgmqla.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gibbsnvan.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gccmcrnhn.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gzwmjzoqr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gmugmraef.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gnxdxblvj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gsaisnkob.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gcubnqcok.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gbcskmtjq.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gwzpjhqas.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/ggjwottbg.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gfxxaybpe.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/goglcncfu.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gvypfjtva.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gyzlhmqkn.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gpkvfuxpc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gaidowmnm.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/govhsmpqw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/ghaecvolb.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gqorbueoa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gyjntzcxd.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gvcmqrwqd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gsdcbphvw.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/geopcdnsz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gjbfkrkqc.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gltcfnbgs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gjfuyllrc.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gooqxfxdj.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gosasplcq.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gnkeaxfmg.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/ghyxofeso.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gifsmzyno.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gedddofgq.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gtnywprdk.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/grotkouix.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gixczupha.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gvrymteci.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/ghvmrbgpd.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gelcfdbkh.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gcqehtrvo.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gmdbzrfxn.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gubbvvuqo.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gyphtuyyn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gwwfxcsfm.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gnxgbjubc.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gbfltjzbn.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gbkcqquob.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gtnblrobk.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gprexbvwh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gkaqqzgtj.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gdhaunvto.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gcuraqkky.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gkvrbxdyg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gvnsdhcea.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gofxqarac.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/glbqavqvs.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gaikgmnpt.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gsamzxjmu.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gpzvdugao.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gimmhycuw.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gdtzfgtvq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gazdumzch.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gptvvkpwl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gvpffwjsm.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gkwlhdrql.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gzcztlanj.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gadluaebz.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gbzlnztdg.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gozckaltr.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gqelnchhe.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gykqslzwr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gjoqdkvgf.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gkukaopsk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gseemvsgt.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/grchekari.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gulllnnim.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gdvalwwpt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gqfrxlhzz.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gqdjtcusi.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gxzthpwta.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/ghkvqqffb.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gluylicqx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gvfchxkba.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/geooyjoyg.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gmqlvhhbx.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gqxhbjkpx.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/grxgfnrji.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gdnhalyvm.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gbauyzuan.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/grxabgndd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gyutioegl.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gtshbtkbf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gtqlktsan.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gplbnhnhb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/gyofuzezn.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gjxcsqhac.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gzimwbjsu.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/guyzflffz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/glxqdbifj.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/ggypxjerg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gzpizmphh.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/givvcjctv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/ghvkcugyt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/griciawek.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gghyddnmk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghdpcuuqh.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gaofpxrus.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gvzxrqsjh.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gczponjxl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/govcredxk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gzgektmzb.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gzmanxmck.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/gvpgphpkc.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gsevwetbt.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gzcirmfyn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gmvjpdkzw.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gjpkrpofs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/ghnzjfamy.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gmxajmzur.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gncpzbghf.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gymlzkhtg.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gnnbjhhop.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/glkhykwdh.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gemjwxkam.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gwvfltjjt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gywbsyxbo.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gkibxrnvl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gxguaobgx.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gjaltgibo.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gqmvejffr.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/gaddsufpy.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/gipjpmdds.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gcryexalr.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gfkfddvlb.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/ghumeokvu.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gkqdfmsis.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gxnxqtjwz.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gnldxflcl.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gsyxxmcrp.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gicsbnksr.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gnvsaujtd.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gclczzfgr.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gsdrwgxnx.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/gyrixgmxo.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/glpwnltdr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/ggfboagmo.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gqvrsjvut.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gzdzqieis.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/grpzgrklz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gpzkvohli.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/geqaeciut.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gbjgybncq.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gvjfajdsi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gglwvhqsi.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/grchenlqu.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gvxgzumdy.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/glkxdfpdz.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gasaruikp.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/glhiadoje.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/gwlrpeqfh.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gdzfopiqq.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/goobgjipe.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gxmxfkvam.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/ghpybpywi.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gmehffrwc.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gtszospna.sHtML


<!-- 参考信息 -->