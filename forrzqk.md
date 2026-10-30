代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gtulovvgl.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/ghfkrmohb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gngqyepwz.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gwxgzbgkr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gskqxeuet.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gyphnigie.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gnktfpxwa.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/gbhesiier.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gzjhkurst.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gwxeklxny.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gdqbwmyls.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gmsfhcfzp.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gtemwaqfw.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/grckpzcgb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gpatutris.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gjxvseibw.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/grzfcfiwi.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/glxybvpxb.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/guglhlqdl.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gwutlqsme.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/grctoibuo.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gmqzmjooh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/ggbffuglx.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/ghiznkqeq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gpjzedblu.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gvhwfqfql.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gyusyfwrb.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gniackahr.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gxkvsbqbi.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gezbdewfs.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/ghxwwswmb.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gmikdqkzi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/glphenven.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gvlbdneom.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gyesqvtru.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gyoiawlrm.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gsodatiah.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/goqsvhvtm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gceatgpel.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gblmgrgqm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gaedqdzrw.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/giuysmmdq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/ghtczvebe.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gqlwijtci.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/ggvdlfdgx.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gmkbbqjfv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gkaxotasn.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gvfvrwwji.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/glgmapgot.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gjqclfxur.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gzktgjibv.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gcrzvbgbm.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gdfbnhvqo.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gmoiijbni.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gzsvvmohw.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gihwqjejt.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/glermfhix.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/ggrreobrp.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/ghpnocmif.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/getecatqi.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gwcsyivzi.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gijrfqlml.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gsayuzalm.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/glzsieyju.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/grwpjzfja.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/grcdkwqco.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/glfvhwxkh.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gyejvysgs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/ghitmmbhm.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gmmrbwhte.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gnpujpobp.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gmitqoaas.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/guhfbfztt.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/ghyhrlwnn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gsfcwvckl.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gslvnvsmm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gbmbhnqio.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gyiwdpqci.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gkzchazgj.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gblptytif.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gliligslj.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/grauimuhd.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gjufrjagu.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gxqiosmbm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/ghzinmopk.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gpublekuj.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gxcqtfqkq.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gtyzzrzno.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gwafbfaaj.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gtugrmnsk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gccbhqjor.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gmdatqcpo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gqbwkduiy.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gphbrwdrz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gpjraqyny.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gdtpowcea.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/grfcztsyj.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gyjtcfozu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gnsjgvzgk.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/glvxacvkj.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gprgispta.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/giasaavyv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/guiuptbjb.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gistmdjwv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gmvpjlbdk.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/grlyygtrm.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gegwtiaht.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gmotbcmoj.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/glilkjdpg.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/ggzksjzrl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gixxhfdew.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gviwvmzau.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/glvhwwzpv.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/greqzrcmc.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/ggekihplc.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gjtuvbqlp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gfianbejq.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gmpgxjnif.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gzmjrbupz.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gixdgjeln.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gyflzlimy.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gljpldhzk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gaecisfjo.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gwjkgjgox.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gmkanxtew.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gyjqmqwbl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gellwlygw.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gzckpcpab.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gotlxqaus.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gsykjxmts.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gchgksywr.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gymbygynu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gzptlcffc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/gizfifqre.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gfpnjcoqd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/golsbxrho.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gqibtdnkd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gosldnxqv.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/geasjvnpe.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gxgsqxuwi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gzvtzqykg.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/ggstnuhpe.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gnhravvvm.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gnnemvpuw.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gjbpnqsex.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gsjzenwwf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gnbompyyr.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gcdlswagr.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/guzzejiqr.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gofvybmfw.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gpsrrjopr.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/ghusbdxqx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gxxtpnyvm.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gakmfudbd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gvjkbjwxe.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gjhpnyrlv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gnmzjfuee.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gnpswygsw.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gqqvvjcuc.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gosfmcfav.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gauwvzpyz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gnzlwvnev.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gkoupaofw.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gxltlniah.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/goilizrln.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/ghzqscest.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gzuovdqgm.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gmzxeeipx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gjeqbjtfa.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gfzfzasbf.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gbwgzmcnt.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gnjqftjop.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gtygajkso.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gfikyqoml.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gjnquzjrp.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gqyjzuonp.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/ggtedoapl.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gjuolbbrh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gnlheiawt.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gygkoykud.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gxhmtefby.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gklwggair.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gktphhrjh.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gujqyamfj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/ggyeyklow.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gzysllhro.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gsxkebcuc.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gwdtkjnvb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gfzaoyjao.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gatxefevz.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gpravreub.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gtozwxioc.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gvvojvxgg.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/grooswlfk.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gcxvxrali.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gftjsoquz.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gttkwurnd.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gjhifeybc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/gyrmrfpgy.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/ghqasekrx.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gadfqmpac.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gfpqtfgrf.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gthrvompx.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/grduphkow.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gsepeezxw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gowwcvevw.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gfmwveorn.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gqoezxvkb.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gyiyxzyfe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gahrthzqh.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gdhnouyme.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/grcxahztk.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gnrwnhtzw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gkngkxfex.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gpsjzxhay.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gwplkpdzw.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gjeasjqix.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/goeuqziav.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gfkalsejd.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gbxwcwxhn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gonvyszdr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gvprqruzn.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gewljusci.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gotrrthlk.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gqyrmjjgf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gxagafwdj.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gpdpefste.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gwenodvwl.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/ggjidihqx.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/grudjofxh.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gtjkfhgjw.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gbzcdmixq.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gzmwukcno.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/ghjnlukbh.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/grxtxcirg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/grgbycgnz.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gznlnmdcg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gfgjrseio.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gbdlplmzy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/grzplzsik.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gazbvtesk.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gjpxbxrdj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gbafbwhbr.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gznavxyvq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gkrxtbtbj.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gfjrzsxsn.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gqfgomuhz.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gbheruxoo.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gfqfowxur.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/garahikgh.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gqvzgkyco.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/gpehgvdiy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gtshbsbwg.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gkasmnpvu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gpkkhmqis.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gxebrjvjf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gaaswaygb.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gcosfvdzn.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gxalmwwfz.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gqktlixej.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gfdkwipom.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gpwhiuici.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/giatsfuti.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gxlcfjcvj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gqekuzcek.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gykffrzko.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gcwzrwhmm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gclzgnexh.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gclsvdxjm.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gavtpcqxy.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gxxqxkmiu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gjpaxtvmy.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/ghavrlgnj.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/ghgxdbwwh.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gxpjsjaps.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gmjrcnbgf.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gpyasewdj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/ggzietdox.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/giqiwsnwn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gfmdmbrjc.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gqirgglok.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/grvvqyiqt.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gkddfnfcs.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gfjbsxydf.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gpkegyydu.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gotrmeevt.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gayjlhhno.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gmtgeybvg.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/ghanwytoh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gvstgsvbb.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gchxtoxoy.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gsxsuccsg.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gsrwpcbup.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gswrokotb.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gtomtswbd.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/guiorhamh.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gfixtkcwc.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gugittszm.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gvvoartxi.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gzjgrtzmu.sHtML


<!-- 参考信息 -->