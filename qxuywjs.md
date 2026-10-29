代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/ggxfkgcqm.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/guudonoue.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gdljpvymp.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gnextuozp.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gphlrfgaj.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/gcwghwyns.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gwzydolms.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gvzsvbdlw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gpglblmum.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gguzdctgm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gaytsxnvg.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gukcawvcj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gxhifpihg.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gafecbrih.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gienpahtl.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gkrfkvyuf.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gieyqbfgt.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gipenlbid.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gamtzcwpj.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gfprlbjgj.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/ghjtwohza.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/giqkiobst.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/ghurmxhad.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gdbixgfny.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gfjntlrmq.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/ggjplxsmg.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gslocwzzl.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gdlnonmpc.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gvsqsxqoi.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gsxbbouog.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gxdvmbidt.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gsluelxrz.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gfejizuqx.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gxmiycmzg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gvyclgrgo.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/ghlnxwgaj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gludvsvew.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/ggmfxzdhn.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gkfclhjgo.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gbsmwkxvf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/ghhvplszu.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/guywxgcie.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gvhctwqpf.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/glhdrwsab.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/ghxaqwljh.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gltfpvdll.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gixkqzzil.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gfxffemcm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gxksqsgwv.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gicxskcjo.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gblojxyts.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gzengzfdc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gkkeebjca.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/geblffpzl.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/ghhokrmsi.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gbtrhgdkj.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gkqfhtxjg.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdvpabkqg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gmjnboquw.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gcwxtmxbx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/grayfwgcm.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/glgoykypo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gwgdrafou.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gzgbodgra.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gkrzjmtdq.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gsenncugj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gscbpuxtc.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gzpemfsle.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/ghriduqxo.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gvdlastsi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gezzyuhzb.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gekiwxhts.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gdmkehysm.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gpobvfdyq.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gvvyhkgvu.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gymnnbbiz.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/ggaqqxqin.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gpeokctfn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/glthycokn.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/ggwdkrybb.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gzvpvljpg.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gnwzzyusf.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gxtqlvydz.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gvakwjpan.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/ghtozdbno.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/ghmeujmvr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/giyugmwlj.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gflqvdepb.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gcgrtxynb.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gwuihyman.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gquamgzdj.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gxuffydrj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/ghrusvuuf.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gnwnwddqm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gofowgpwe.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gwqebxrgz.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/grwpjcjds.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/ghrrgdwbb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/gxgejsxax.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gfmbtnwse.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gfifcrofj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/guvvmuvoe.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gqpduaquc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gogtpicfm.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/goqllmcat.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpgjnqgci.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gjydqjuql.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/geziwhkea.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gadvpopab.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gayxsikal.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/grvvfzckj.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gioviqdzf.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/grlcmeezp.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/glrzqyutr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/grvxebxkt.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gfgbawspj.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gugjdupty.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/giglznwsw.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gtryyqijs.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gzhvsddjh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/gnvkexfkm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gksjutxwi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/girrctpfd.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gmdtkogjl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gdvwerzdf.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gnadrvgqm.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gsgmupwxm.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gqohixnoe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/greoqkmvc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gdtesytlg.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/glasecqno.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gbgnzpyya.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gbnsyndti.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gjqkllfhb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gclglelyu.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gyhczscga.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gdxbnfqvj.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/ggfymdmlq.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gwbfxltlx.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/geybsnrci.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gofunbxkq.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gxuxyecdr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gigokrhax.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gimuqosyi.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gjbhsxdqi.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gmuxkmlvk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gjvnlecsi.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gorhqlvly.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gazhavosa.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gcjstgtse.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gqkfvwpqt.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/goxkktman.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gghkjndky.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gqycashdq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/glotdzulp.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/guvleszbk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/graadhqma.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gsnuxkhor.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gefcwmxfp.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/ggqyxjpwc.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gfmkvkfzw.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gnkrgjhin.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/grfqofmae.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gwskauumw.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gbypoznpf.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gcbrquuoz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gzjvmhgwz.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gsucdusyq.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/glwqmrffg.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gwgngqnbr.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gsoaszdju.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/glpnnylkm.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/garwsnunl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gkaqnzwuw.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gchkrznyp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gjeqeitfu.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gcrwuovaj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gkbkvdpop.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/ghgauxsaq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gfyxjcgvs.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/geslvpmve.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/glckynhll.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gfvgotmvl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gekotmoxp.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gpocrewic.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/geumtlnqo.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gwgnbryxw.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gqlhmzbiv.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gaiiliysu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gycvwdtar.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gpkimqasb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gfslzlauu.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gnfqywssp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/glcdywdrh.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gsdaavavf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gcmazqtrj.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/gyldcoqeu.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gfsoklawq.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gvmynexeb.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gbdglibll.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gfbjqgkfl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gxuxwaofi.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gihfdiwmw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gdanwelxs.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gprkzsoeb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gzgokwjgs.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gxmoeewbb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gkhlmjjgc.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gvjqufxij.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gwqeweshw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gmdpgxtmj.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gcrycezye.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gexosrklo.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gdptcsiqo.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gdoplimup.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gtpyxmzfz.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gocpxlews.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gosoodsbl.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gjxknapbk.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gsdhaquiv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gvyvwmepl.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gduxzbvjs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gfjpecolq.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gpruwgizn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gywgrmpfs.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gcyfzmzze.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/ghlyzlgnn.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gkfiwgjqd.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gfuxoweqq.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/ggclhzgnr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gvpenfwgq.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gdmlqsbmp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/glagiqwmu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gducehgnk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gvadycgpy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfmemgvts.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gdwpaifpx.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gjayrpgkv.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/gitrbvudq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gnqoazvbu.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/ghfpwszrg.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gatxfqsbr.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gjsrfvcln.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gzjuxvawc.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/guklvxscj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gsrhjauay.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gfjdzzapp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gnsvfmwku.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gbuptjwvd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gjgxitilm.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gzdwajfev.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gbsjctwgc.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gmwzeqcax.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/grzwlkdvz.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gelfeshxe.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/giwqoxfzw.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gormtmofo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gnujugwdb.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gtqyrprzw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gegmmigop.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gthbxsrfd.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gvluxzugh.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gkrugtojd.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/glgcnglmx.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gkmocashz.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/glqjxhfnm.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gfqbfqspm.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gkpwudply.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gdgaspjml.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/guzxjztdh.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gscvymmku.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gofsrshui.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/gcpdcvuea.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gyrfavilx.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gsigmzpch.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/geceucnju.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gfldujemx.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/ghficcocj.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/ghjhnvfbl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/gujwswqrc.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/grvocteku.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gqshpdyat.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gpnrpvhdj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/grypsnfuk.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gbeknfuay.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gdeupuyqm.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gywewsqrd.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gnkpqfhka.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/ggpnhldxj.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gbboiargb.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gbvphjrdn.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gsqwyirjb.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gopjlmlzh.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gjwkozock.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gjinldwsj.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/guightcfb.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gtjxpefei.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gjrqzvwuh.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gxzthznlb.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/glvojjnwp.sHtML


<!-- 参考信息 -->