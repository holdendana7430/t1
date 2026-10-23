代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bhxlxqyp.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3liilfsdr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3kdlwlvzg.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3kocczdtu.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kbhvuzjj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3letwckfh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ojuvwbzs.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rgpejoxu.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3rznwertj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3bcdgnbyl.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3xeqhshlo.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3opyjnppj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3fpsefxmd.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qrdfpfbs.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3fwiqddin.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3fmjwaezr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ueovssds.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3admqxvja.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3yrezljmd.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3kzoapowx.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ytphpqos.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3yjuqumxd.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3gkwcjyrk.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3yukgcckf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ilpxumxn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rxaoeutq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3dzdavkiw.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3adcjlqhn.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulzvofvq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3txopqglq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhkauhwp.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3hvmrxemy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3vuopewvp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ymtsdzia.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3lnmklfzp.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3kmeymjlt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3loyaundi.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3xulaglfi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3elnqcjuh.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3jdcstnqp.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3vblfgwlm.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3bedwklli.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ullrqqly.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3otnwqlrl.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3exiivrzx.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3tvnjxjth.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3nkszxqgu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3jktpxuft.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3qkpwtoug.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3zsakltix.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rolsrhcx.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3txvafygn.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ufukpdzi.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3cmbmjjzn.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3uigucwzc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ipaxjrve.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3meryxhgp.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3vgcikhqi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3pjanmtuw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ornrilwi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3aymgnbsc.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3kevzshcv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rsjvbiks.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ccanggoo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3sxptvfvi.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3odakiymb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tsrmbcgd.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3txhmzhrv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3bpwktkgd.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3fidmsosi.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3yrdtruxn.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ltxnadmo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3fgnnvcek.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ghsjmyhs.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3bcqgdqsa.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3uidgxcuf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3xuuqqntq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ihebizji.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3vbonnyze.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3biqdblpo.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3phhonrib.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3gmnvojaf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3irwzqdzw.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mqjqbnpw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3jtoxikzz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xulwovqt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3xnryjcij.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3kalmswsp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3rzjgkxvv.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3cljtycas.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ugdwsxdk.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3hpvdszpb.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3fdgkrbel.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3rwjpvquq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3tiubjgip.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3vyjlrtee.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ikdicsow.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ywoagsvm.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3sdzeaqhu.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3bqmbcqgz.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3lhkpfhti.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3uisewjdi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hgzuybau.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3cainwvbc.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3zsihjqff.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3tsvbfppz.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3cgwcpoff.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gvmhwwud.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3mjdleocg.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3rknaunhd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fthbjxou.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3wjddhjfe.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3bzgcvezk.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3pgutamvg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fbvwoovs.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ircsiwlk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3hevqscaq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3mgyxpxqq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gowrcxeo.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3cndhounm.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ypwvmfoc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3zrhklhie.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3dtpuisvh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3wbdhrycp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ueievhmk.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3nblydkpm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3umimpgnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jastgaiw.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3eftqoagj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3urojenfp.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zwknhqxz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3rongwsqi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3hojvmpak.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3damfazro.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3yhxcizhv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3kwxjdzap.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3qlpyhfoj.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3whblaqrk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3yzkfzwiu.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hkqxhzgw.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vqyhwytk.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3llzfacny.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3idmwggqe.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3gdfhokqx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3lojwiyjp.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3rvavotte.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3jbyzrjnf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3bnjfzlhu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3fyotknut.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3tdziuxte.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3uiwrxfxs.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yttsurpn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3dglqkgfz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3pyfhqfhy.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3eisamooj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3bwmvbfku.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wsjsohdo.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3lfstjesx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3jcxcraqx.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kfzvdjoh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3xotvists.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3xbcidlap.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3imfrzmgz.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3khekbppa.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ftvneasp.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3miwksflf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3kjnfxdpi.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3wshfpubi.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ofdyyovt.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3qsyvkwae.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3roujkbbg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3lfpbkqhn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3bcdqqanu.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3egnczycq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3dzzzzvhf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3aauedeae.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3lqvqbcpg.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3otnskuec.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3bprnrpwx.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ayylukjy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ebdlppqj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3poqyaceb.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ysqjqltp.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ndxhnjws.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ztfofgzn.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3lewdwkfl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mnhnnrjk.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3oqpjwery.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3unoxlxjn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3jertbcvb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3nnnsowkm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3wkvfooia.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3omohajus.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3fyldgvml.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3vtkqbwfz.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3toaolrzh.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3dpyqxfgb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkfaefbv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3vohnlzpm.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3msrslalb.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3kkilsrpl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mxjtmblr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3fntqqfyk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3lqomizcx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3qcgrydml.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hqicltre.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3gxgafsrz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vxkplxmo.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3xbypwgzt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yknvkcyx.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3wkkvgnji.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3bjexwysx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3yvdubyjv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ianlysem.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ghrbbhtc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fmavmlkt.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bkwswppu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3xnatgnnq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3mlipapml.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3qddhxujp.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3easbyzps.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3gchbkyfu.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3waocghcx.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3zyteuwne.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3xatdfqxs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3qrbljyar.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3bqpullxb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3zwrzlvrj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3mrrbwjcq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3xifxnoum.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dzqzeavd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3zvnzqvqg.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3fvrkfsfa.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jkafppct.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3mzmcqqph.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3lniprrwt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rndknvfa.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ywvipmxp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3drzbuhmd.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3otsxched.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3kiuzxewh.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3wrngjtsu.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3iyifxvfe.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3hwsbwlwf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3xamvwcpo.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3wulverbw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3rfcisjvs.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3kwngeddy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3pixeryzg.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3anycgojk.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vvqmxeuf.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3tgygozdk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3dwfdegoq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3dvrumkxk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3wenaivyf.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3fufrdwrm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3lysbkvyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zynidwvb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3uxrrtxaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gwtmjmyi.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zdhzqbrl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jyentrev.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3vstkroze.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3yibstvml.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3xkeznwlv.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3yeovcxmu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3rwrtjmfv.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3uazikrtg.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zvvyonia.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3cxnvnoik.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3pbdzwawh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vurnbula.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kiwgnxid.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ctbcrnfy.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xwtiwotl.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ucxevqgt.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3cvfxlmkk.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3smgtifve.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3rpdojtwr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3fixbicge.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3bsdvmhek.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3qwdovfij.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3iiatyipz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gvvuzdpg.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3vbrggszv.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ovsjdckh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3sxonjqhe.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3bkmkgiei.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ircicxxy.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3zggldcbp.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mdmfaytc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ehqqlryb.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3jtgdjppg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3acxbjquu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3eqvrlkcp.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3gwqisclm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3gnfjtcds.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3gihuynaa.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3fmjypmvq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3gefllvgq.html


<!-- 参考信息 -->