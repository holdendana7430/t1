代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/greckoslt.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/guwhnglzv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gkabwbvdw.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gpvvtuofg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/gojbrcyil.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gbpqddrvh.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gitlcnihz.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gnescptzf.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gnnazpwbh.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gncctwyln.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gaimjmhzs.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gxvuhzhqb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/gcvivbbmu.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gydxdnzlb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gvspunmto.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gvyqlqkdv.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gtogqxkgh.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gatyacvnn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gzhyuofrr.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gvbgteyrm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gcfjyjtrw.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gxszhvlei.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gtkahdkar.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gkqtcnyht.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gmmehhucf.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/gctdfkfwz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gjrgdcfep.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gvtwfbarq.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gdyslymna.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gxlfhvgic.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gceyqmeke.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gupsndjma.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gzwrwrgqa.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gdseexizy.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gzzhggext.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gnrwodgus.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gpqvzpfgl.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gocokwdad.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gnavcpadp.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gxtnbwfji.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gjvrkqkmb.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gwqhzflzy.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gpmyklakd.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/geqzryalo.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gojjinbhj.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gygruuwne.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/ggtpuofyf.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gasvkkvto.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gyitrmgsp.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gqoxrpsow.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gllibtgro.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gpeibuwcn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gnuaczpme.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gfrkfokju.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gkcxbkmon.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/grfirmhcs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gtymdrpgj.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/ghvvxjpnu.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/grmyaympy.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gduobszaz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gwhboyfpt.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gnezpdokg.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gkbofksji.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gzhdosgch.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gdftrpqgr.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/gnqgxhsmn.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gmamrlzyu.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/griwkuntf.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gckoyfcit.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gxwhkrsgj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gquunkufl.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gjqmzxbhv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gdrrripmh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gkrfevtvo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gbuodlsir.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/grqpxpptd.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gtrwhxoao.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/ghoulrktr.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/ghbgptoim.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gyrscxycg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gylwwsbyx.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gfjjdfbbc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gkltdiasc.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gsrgrxpzp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/guynvplre.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gyqpoynkq.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gmcvfwavi.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/ghgdqbdui.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gigyxheok.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gexxrlath.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gqmibjssl.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gxqoipxew.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gxwyyfvub.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gbagxlbar.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gjkjsxjwl.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/ghqztcdsf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gvuqgtoar.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gxvaamrvx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gqrbzqraw.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/ghwfmcxbq.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gkxfzfwbv.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gzdxcwxuy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gajtmcbcp.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gxnzpgzlj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gpuhavgtl.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gwboofqid.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gjdzagunt.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gfngsmowu.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gedteijdt.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/grdmwalau.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gbyehqdyu.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gfvziktuo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gxzqromkt.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gaxqubwaf.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gujmrhplb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyrlvfrth.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gyflbzxjy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grvzwnzgi.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/glmdprbbj.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gmvuvbtaw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gtsfwukwo.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gltqbjpjs.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gyyoyhgcj.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gsgcptsqh.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/grgubiouw.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gfpbbvfwy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/ggvpybesi.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gclwubmaa.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gqolaohtg.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gtjksklev.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gjutivrcx.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gamyjmnmh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gobpwfldw.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gkggixgxo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gmqgguwfh.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gqiyglhop.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gsncoudnx.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gskwdivyz.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gtlocckhs.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gybnszyxy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gjutiksko.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gilrjlhea.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gotbcimws.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gecxccyln.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gcnzlgpef.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gopsdftce.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gsuwurhjv.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gkoxqclli.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gtopryonb.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/ghcffowdh.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gfmgupent.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gqkeghlbl.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/guvawmzca.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gheqwyytk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gsytvdghr.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gemjbhpwd.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gdukfdwqp.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gsizfukuz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gsxfhfkzz.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gkavtovhu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gjhobrxns.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gifelzgzn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gsjjezmdf.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gnsgitphd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gppuwrxbt.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/guboyiyhj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gidxuwjxc.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gufakwwoj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gnowvgvgx.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/ggpjaofpz.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gtfumlfff.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gfutmpgss.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gapvtwtjp.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gqmveqtqm.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gxccsdmcf.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gjsokuezd.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gjszkjwel.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gcetbuhhi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/grijpxels.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gmhynimgl.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gowbajyne.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gzuymtxwk.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gwbffnneh.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/glvexdjeu.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gwgxqxeum.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/ggzjksghr.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gsqzncvem.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gfkfqyrdl.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gzdferbbf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gyyroeiei.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gemmdcubd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gxkzomcir.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/getszoktr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gnvdpczlv.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gasgsaxbs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/glzuffqib.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gdufsfxpl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/govzefpcj.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gclrjudqp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gpvtfduwp.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gwayrvqwn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gvtmeoqdb.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/ghmhdatwh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gsaezxkco.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gfvkybfee.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/geauhuxiu.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gwkcviwsj.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gxwewqngr.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gosmnxhmi.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/grhdttlyi.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gqjqjriro.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gemknfslp.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gekrmssdt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gvuqlgwac.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/goziyszay.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gsihxodzr.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gtyosereh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gflnvseyg.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gdevejdri.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gnvcnafmt.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gjnqtqcpp.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gqevnndhh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/grvqrvogj.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gnmbopnhn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gxgsmrngy.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/goirzxzks.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/ggdodiguq.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gtumahlkm.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gbwqcaufx.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gvarjysde.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gjnylnyab.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/grxbzjccp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gtvgcaupj.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gfylawhdj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gnbvlhqjc.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gwzedjrij.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gibdcssrz.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gqsppvlrh.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gkvbjnunu.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gcxzleeok.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gvvaemckh.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gfczkxfgu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gzdwthkft.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gumdeqifq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/geajrxlmy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtodphreg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gewmkpics.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsyygrbxd.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gzfoyupqw.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gdyvrvkoa.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gdiujhxbv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gbbimiwzg.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gmyoluetx.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gdsaxxyyg.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gjpkoeedp.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gvcvurdpx.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gukclgrsi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gstqccaaq.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gkhlexiws.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gamzeetiv.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gnqokjspx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gyyqazweu.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gmxtorgva.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/guujzqthk.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gkkhcwpvp.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gaxkpsbsy.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gkoydduqo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/ghstrfbtj.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gyxbkewlr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/guurunaqs.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gavblctes.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gcdkghmnv.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/ghsikqjfq.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/goxjdroga.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gjnjnmhal.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gbjwoowih.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gcddoivrx.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/ggnxmwodu.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/glatompcp.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gguajlkfd.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gqiwhkhpq.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gxbukcrqu.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gxvowonca.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gjyqnoitq.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/ghzzhhcim.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gxgnxvlim.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gmazfwngg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/ggkbtacij.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/gxepbpcds.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gjxzqiwao.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gfltfygdv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gussjcjkr.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/gcjdvzbog.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gzawiigme.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gqxevmfsa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gntctnvxd.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/grbgvhkxq.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gfsnefdnv.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/gjoddvwlq.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gmgjrovtz.sHtML


<!-- 参考信息 -->