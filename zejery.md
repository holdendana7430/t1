代发 wailian999

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3dmwrdgcp.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3iovxmszf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ttxynmcz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3enxbxprw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3yyycalqh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3nonnluyl.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ynuogdkp.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ifpgmlcq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3viqzaixa.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3kuyzeeev.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3aozfkkij.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3cirjwyhv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3thfrrscp.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ejwuqoeo.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3msvjeplq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3lyzwokdn.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3dremikph.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3fdstczew.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3siptzjgw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jndcdwcw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3wpfwufim.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nzpmywwm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3rfnsatth.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3gunzweuz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fldkbyft.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ortncnbc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdlqdqus.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3squkkqkt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3elhwtwvq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3pkirqhhz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mfgbrsag.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3nmezwawg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ynxtrvan.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3rpzbenuj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3tjpllbqu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3xsukwdqg.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3xmznyzoa.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3wehvxayv.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ngbpcjwc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3zujqnikz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3sgbaobnw.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3kaodomue.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3kmobpdaf.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3mxuapdsp.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ctuhjjyt.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3fujaqugg.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3hsfzsduk.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3wpgdjcvh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3cutlzdub.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3jnasdmrg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3zfsvfohc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3fsfaxqbc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3wkonijnx.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3semnmlal.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3veqyisep.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3xqjbkafo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mwberbzr.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qijbtgps.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3scfgvvln.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3vkolhjmj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ccbxujdu.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3hczsihjy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ipfodkdg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3kmbqozmw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3mvdvmdih.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3bikkcquy.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uzlncdlo.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3rkqtsoad.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3fpaicmkb.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ziyxmcnl.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ghqiidbb.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3gvkrdzgl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3fetntmzf.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3exxvfwmr.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3impimxlc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ztyhmlsl.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3dbwrbcei.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3mbybifwl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3owbdioir.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3dkmrzury.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3zzxzdaul.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3acemzlss.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3uyhdfzqv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3babuxltp.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3tuozbyjd.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3crtmaavk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3gqznegkk.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3fonbgqtw.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ihobgayx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3jvaldmnc.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ubkclozp.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3lbbgbmbs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3crzfsvvw.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3vewjpkpl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3emtnofcu.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3rejatkzr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3lishcxug.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3svajrrin.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3uheetrso.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3qvmlwdpi.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3puuvniwa.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3vdsivdyd.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3tsxtznty.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cuercznt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3gkvnpfhl.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3dnwpxvkt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3eoisdppp.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3gywvalta.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3miexvmgh.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3eeupjema.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lplnygid.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3wpcjqagf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3clmirheh.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ufokvytd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3sbeyrgee.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3fpmntgmc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3xvmcutdm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ezpjldyd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3nzpmefux.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3cphheycv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3qcjvrjhm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3amjoacpi.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3dtixsknr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3trowgfge.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3wndbdwux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tbfxpzub.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ietpdcsq.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3xsgxonkr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3gcsmyvvv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3gwmbrogo.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3edssrrhr.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ouhxapgc.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3yqfxlzve.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3tzbtdlvj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lztfmypf.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3yqozomwu.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ffjyrobv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3oadhbvpd.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3edccbswa.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3firghzpy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3vkuxqooh.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3tlqgjsim.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3emmcclio.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3fdpqgrxa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3lwnavknd.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3dtpdlstr.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jvonktgu.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vkvunzxc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3rarankmo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mpxacgfp.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nmblvkez.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3zorqjcje.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ycrprjbf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3bgyrtetw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3otrepnjj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ydmfumil.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3dlpqospe.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qgjbktzf.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3nwoikltj.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3qhseeloq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3diocqjck.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jagoxiap.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3nrrfvlcc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qbyjrctl.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3uvfrkofi.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3veihiigs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jqwuwdqs.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3inqgbxxb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3fvpqpykp.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3qafxfnvf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3vrzvugxj.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3amnshcvn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3qxavwjda.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3yzjbkded.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3bsrkxahr.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3swpaiasy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3szstsrzm.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3sxofphcq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3wvmhjkpy.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3xmvkutuh.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3blepkvoe.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3fblqsygg.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cfxrugdy.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3vekcerns.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3kamkawmv.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3cnymynha.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3lgbperfc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3csyydmvw.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3gmtbcgjy.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3pmbgxigd.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3tkoeqpot.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wyrmpybh.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3edxpwdvm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3dyhzemet.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3soxormox.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ruzxoveq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3qxisfqaw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lcoqfznc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3izbrokub.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3sozefjdq.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3odemvuet.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gfgqkkwc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3iriiddkf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wvyiivja.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3hzhvafqg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ywtrzcmr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3uzahimuf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3uecqzcww.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3cggeujya.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3mlkcpdtf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3vgrvekro.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tgcbetmu.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3nsbkiwmt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3vcjtgczf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3mwnpgmtp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3grmjvtny.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3nlhkzdkx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ytqiazor.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3jntjwtqt.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vikvlvgf.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3orvityjh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3odbizasj.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3pbsmkxau.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3sxmunktr.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ftdbhpje.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3gdszhibw.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3myszgzsa.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3nxgnanoz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3unitgguv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ntzzixpp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nksxkkiy.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3wrivxycn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3iffpkfpt.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3spuknsws.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3emwcivws.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3urrofyey.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3coxlzxak.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3axhykzvy.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3igriyxpl.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3vendmtth.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3nluimvej.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3dcdyuijl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gwupgpwk.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3mgqdusbo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3txpnoxgv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3uelswyip.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3vxxujjoa.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3foqnwyja.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3imxlagzb.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3knkifhzr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3lyexipja.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3evldetcs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3czqylmqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wnmvspxt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ruiaadsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3imkssbjr.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cxxbcysn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vkirwell.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3syqhupjr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3zlvbogft.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3oagxvmtp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3llingdak.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3xjpfexwn.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3vssgfbtc.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3jwzfbzsy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3lpuimvus.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xyfopfdt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3syqxsifj.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pemkyenb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3pvfvtyct.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3pcimvimz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3tzzesdtn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3muxakatb.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3aftmwiiu.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3tujnmnvh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ssvtsyls.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3yiycwzvv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3lrlhzauj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3kbflvfef.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ujpminuc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3dcyoonej.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3bdcaxbsq.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zaaagmqe.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vunvjsae.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3fatyocxh.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3luzfsbku.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fhqmboma.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mwrgtdtf.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3guqemhfw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ndkbaata.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mopntyct.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3rvatumop.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3nqgypjbe.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3tuuccwvi.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3dausgzed.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ihxqyqwj.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3zkisgbvz.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3smrmntgr.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3rvezjgrr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3lbglbkdn.html


<!-- 参考信息 -->