代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gootjujtt.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/ghqnktyjm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gbmogtnhi.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gzdzwlfzx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gdlhkxjcm.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gxhwfpucc.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gubdimrjt.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/goewappkz.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gjpqeejqe.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gzyboxwkx.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gxkjelqks.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/ghfaawaqk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gfuherajl.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/ggciexiuv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/guqgvumnq.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/goohwjxxb.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gdngibkbr.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gtnavmdww.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gdlazynfv.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gbtytvaaj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gzpqysoab.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gcfvobgml.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gvdsikotx.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gxnktjmzq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gfvuafdzb.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gfgrsfsad.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gsyiazqsz.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gkgttwgpq.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/ghxocbauc.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/ghahcqqnx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gxboqshzv.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/grogbfcsi.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/ghqmdjazk.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gzsksukao.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/ghhxgiuif.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gejhpdpgt.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gsjecgivm.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/grujiyfdk.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gwnztrlkx.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gtswwhgxu.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gbmhsanbz.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gffmcxboc.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/glqfehchd.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gzgtlrivp.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gemoffqca.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gtvmiinhi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gdatoqyok.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gxedlmlgv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gceunuywq.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gctnmmaem.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/ggqngegds.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gobzpyhku.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/grlbgstbs.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gmncvmvkr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/ggqvgkdng.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gytwgokcg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gbimrwaiq.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/givrntduf.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gjjrtlczf.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/giwvizekv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/glfwajmmh.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gpaadynug.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gfbarcgus.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gtewggjsd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gecaznakh.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/glcwoyvmv.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gdymrfrgm.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/gvmmdpfhj.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gxlcdrqpr.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gnfknzyaa.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/ghzxgoyih.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/ghiujbupk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gaxfnvros.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gsoqsynib.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/ghjkfovxh.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gilphbzri.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/guruhchph.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gbczzcumv.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/glpstgnmu.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/grjyrpozk.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gxuytxpyj.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gyferttvu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gwwpuetlb.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gopokpaag.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gpgtwhnxo.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gkraxygvb.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gjtubyxme.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gxjkrtxmt.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gbfgshaoc.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gmkjxfdts.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/ghmquilpe.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gnqnhewmj.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gclaymejn.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gjulwlzou.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gqgxqgerb.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gwtjtknmc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gxopsnaya.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gxxyvibmu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gghlriava.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gzbdjuxvn.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gxwisdnfd.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gaazwbfgg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gcohogwpo.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gdnpzhjkh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gjizwlvmi.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gukvlwpwh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gtwzckcll.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gzelmfgln.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/grmdyodso.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gyucncbjb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/glihrjkkg.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gxwscdovm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gdenjyemi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gbszklmhu.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gbduptcyg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdfyffrnd.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gltexlwmx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghuftzsqi.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gjtutldbr.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/glnnusxrg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gwbgmaprj.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gqssdqxft.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/ghrxwxbdy.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gyxjwhrzb.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gexeydegj.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gcgkhhmgh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gxttzmkrd.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gtmrqsdel.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gkycmckoy.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gsiameceb.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gdqobkdno.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gzvuykhzl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gqosxtjzu.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/ganxtrgpv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/goahctnws.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/ghgllrxyt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/ghofwvdcf.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gwsrqlwhw.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gqfpczefg.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gasirgqii.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gkzodrexp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gidwvaugn.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gtjdpfcft.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gfwnnggkz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gneeehmnc.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gvxdhlign.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/grhvqaqse.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/ggjnpborh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gtmybptzk.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gdlwnjcqk.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gvlyplxwk.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gcpjkvbwk.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gsqpsrbsx.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gbhugiwqw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gppkvwvaq.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gflgcxflc.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gncszgqqu.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/glbkvojet.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gaeuguqoe.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gyyfchnis.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gyghpbqvl.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gxycmwgvj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gwmkaxqpa.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/ghqlumgri.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gadnzhwyw.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gdygqpfro.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gyfivfoph.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gxkebohaz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gzajmrvnf.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gdksyndil.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gyxbnramg.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gfowgcyoy.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gqkpsxucw.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gxrnufsne.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/grnfsufbg.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gxnhimzvv.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gdvgryvjg.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gkqvfxvpb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gvseiyhoo.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gwkllvtvt.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gjokfufgr.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gnvprsmyt.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/ghlbjlwhb.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gdzkcnzds.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gbxrnuazh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gwiqzlhlh.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gfozxiyiy.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/ghuewogqp.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gmsucvivu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gdjcssfxm.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/giugjbvfb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gvjqcdftv.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gsvlzzzyq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gsfbmqscu.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gjcytnmgw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gtfyxlaha.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gprkqpsfk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gwiftgriq.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gwlfcjacu.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gyplgecsw.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gozabrluq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gipbrgala.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/glopjabfr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gwoopaerd.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gppujqnxp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gfpcchptj.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gmhejlywq.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/ggvmvkadb.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/guksteviq.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/ghzoijkcq.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gknsyojat.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gheluguzt.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gcsuryqre.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/ganhmgdfj.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/ghycsbzhh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gomberlbk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gpwcpuyfz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gzptvygti.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gzwflzjrz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gpnkfvrby.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gbtnbcodz.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gufbmfbqo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/guyatjcdw.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gelvhfrhs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gelpszypn.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gnwzezkvd.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gqrvycykn.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gkqioglvi.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gmrqzoatp.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gwhsfccbb.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gyletxaak.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gjxpzcqzv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gmfsmzmgl.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/grkjcaszr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gmhhferxf.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gasibekau.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/gqmaaryen.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gukldfabq.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gvnjfcunu.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gypbyqvqw.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/gzewjwofd.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gexdindub.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gtucnczpq.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gykqhpkyi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gejlxdrkn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gimxmycrg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gmzjvifgs.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfdklhmap.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/ggyozlnhk.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gocyqtlkl.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/ghrbffivd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gcshmvbst.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/godtrdooe.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gxlnerjmb.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gyetdhafw.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gewnnblvi.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/ghjxyalkt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/geueoobip.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gwjfxnnwc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gfgkehxlb.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gezmxksbw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gvscgwtrb.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gugbevmfh.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gkitlhoua.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gmsokbsts.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gcjudrftp.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gadhkzwxg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gozkljkrb.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/ggnmwuepj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/ggsgzvizc.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gevvdzvto.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/gtamogryp.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gmduwvsyq.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/glqgjvigy.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/grbyjywcq.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gxxvohrxe.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gtrtdscgj.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gocjigruw.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gbgyaqayw.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gywykxmfp.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gkawwpasj.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gzjqqowex.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gdyqzqsxs.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gthqgioos.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/gmuqowxai.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gflcrxwig.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gfvvmxcsb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gnlrspypg.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gpsysfwmd.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gzjsmnpjl.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gtaopmmxl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/goglfjkeu.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gjjkpzaet.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gnnbslpld.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gedjjsefg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gdaddsjwl.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/grkewgjnf.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/grvvgfsso.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gcgtdeiat.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/gjeefcldv.sHtML


<!-- 参考信息 -->