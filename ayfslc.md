代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2uskofgub.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2rcwlnsce.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2hptabtzf.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2yjbryywn.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ogfmnnqo.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2whkuugdj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wsybuwna.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xatfxzkh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2lmvozuiv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ekjvifex.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2wgfiwdph.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2nigxyqdy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2eptfqncx.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2eoipankb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zowphyrd.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2dvubwanp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2otedkkzn.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2izhwimvq.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2dikgflho.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2kgiaynae.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2afjtmvjh.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2pvvmydct.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2czzmwtvm.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2uvkzwlwc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2kxcyaapn.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2pzbjdklz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2dudfbams.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2jzelqkcn.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ummnxfen.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2tpkgudca.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2tdjgkzrn.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2uuwwchqx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2tdtkbmsw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2mfpcptyb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2csjvnalm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qmfizexc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2mqkitdrf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2oltkzwlj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2cuhxmfaf.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2vwuipdhg.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2cpmjxyka.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2agnybncr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2eksrmpjz.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2yjgksgie.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2uxefggwc.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2qaxubzdf.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2vvpuasij.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2zxpelwyc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ohfbiykt.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2brfsxmax.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kmnwpsxg.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2vfvovdct.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2whcafhou.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2wjodovth.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2skmvqaqx.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2islhqpci.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2vgjgxxby.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2neiejtdg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2iduwdpsr.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2swzlhsqq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2thtpinly.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2aptngumr.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ctlgefuv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2xoqomqwk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2kmwjgwqb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2inuacumv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zlvsffba.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2vgjojjkr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2lncqtipv.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2tvysiqth.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ouqrbtdw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2xtwccnps.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2rfvsrneu.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2njrhpdah.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2clucghbi.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2gvzssqbs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2uvbdnbve.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pkwoglsh.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2oueuctax.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2znphjdax.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ectvudbp.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2radhlhbn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2palgaqug.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2qolyjpfk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2edfjczoh.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2jdmkzsfb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2hutrjzfk.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2tpofwawy.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2igfnrnoo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2xezrlvhx.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2diffjjnk.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2mlwwwzof.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2fpieyddu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2mbpqjzcr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2xelbdyyp.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2frzfufdl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2zorsfomn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2oaobqagk.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ovjqmqck.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2gcwqwrze.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2itwpatuh.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2yfqghawr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mifecorn.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2llnyuqzs.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2uvpknwlm.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2xripobrs.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2qeefzekx.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2rfbzhfgi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2usrwxqla.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2rbunbzxq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2vdbmasae.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2mrdlanhg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2zrtzsrir.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2hgdbttrw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2dbbxpnjk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2khhthztn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2xhubkflz.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2wqttaasm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2fntnaybd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2boouitha.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2qatprvzp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2tyxeeylj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2bsqvidyn.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2dvmzwsiz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2rtklcojq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2vavyilbz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ttdmmkxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owvaarol.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2pcunsgwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hbjrzkto.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ckojrdgw.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2qvejopoa.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2jiymivpk.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2axtcqajq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2edazknvk.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2wjlhkxey.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2feumlcrv.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2knyitmbj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kzrskwqp.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2yuniongt.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eiahjzng.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wiqpwkdk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2gnudichn.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2olfkllyr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ilxcrtpj.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2wzgfkdns.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2sjyirbht.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2gaiumrzx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2jsikrmri.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2jspzlagw.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2cmlttvvk.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pzuffuzd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2guowflrr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2aliecqkc.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2hjogkvzu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2kwbeecxa.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2opvktsgn.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2hbxalcrn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2rewesfbx.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ceazgzrf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2udnjxbii.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2odxfdoft.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2aoiczigy.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2pfwzjunu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jomayive.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nypykajt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2xjlupsmy.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2dyoncmls.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2aspftpby.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2kqktoemz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2cbvexmwb.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2kncqdail.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gpxaffsc.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2dlikryxe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2xnvakklp.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2hstfxegt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2fynhddzv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2lrorekhz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2tzovutee.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2dkjhojvk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2lcdvtjgr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ofexhaam.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2gszbuzbh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2kqjvwzci.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2nkgzkbjx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2gxjjvaib.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mnhxynpw.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2dlwkwdpf.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qihvfoqz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ssvnkvgd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2mhqltzku.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2cfwcptvg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2qnjruimf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2motnxrra.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2eilkisad.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mluxzxkm.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2bvrrvoww.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ugkkupvl.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ftfbehuc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2xvswicpe.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ekcvybte.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2nqmgxzsx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ezzkcjic.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2thylgehn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2arkmwojb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gaszqtkh.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2szpdttyr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rblmndbb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2zyqoogyi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2csftrial.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ukezidoz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2begtlmxm.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2yqxttybb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2xhsssvba.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2evcflppy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2arriwmro.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2iuwsuips.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2pkjznsts.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2dpedmdzf.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2yyswsaxg.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2yunfjeib.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2xkkyogxu.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2gaekjzsd.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2absnrstz.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2svlbllqx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2cwmwiwmh.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2nckiqtln.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jujbzdna.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ogqlbpts.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2vhyrnqws.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kicepuvp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2worjtafu.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2iqejdmks.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2bsttdyxl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2dghufuvx.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2sogwqayk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ilbteejd.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hhkirquo.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2rofpkmqy.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2oyjyysql.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxdopgny.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2cxtspuhc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2krspryrh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2hsccknud.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cqibqyte.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2zhpgdqbd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2xcupzbmr.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ognutjks.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvoitnxk.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2lsppocyg.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2zhlrazcn.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2dlnkrqyf.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vnaulwit.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2miunokea.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2smxffjsr.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2kaddlybf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2sapncejm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dlfidppl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2huntlnwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xnefmgst.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oiqzgdzz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dascleyo.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2pdizwtpz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2zsyupmgr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2qdmthpdv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ugaxkxtd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ixqqgcgy.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ywfdokou.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mzopjnfu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2yoncclrv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2evmgfwxo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gxrtcfio.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2vlkqtkve.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2oyxbvxej.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2nslgiryp.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tbabxixm.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2egiabdlw.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2svptttvj.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gsqwciwk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2hbogslyi.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2znlogtxl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2onfqbrus.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2sfgfffcp.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ryyocbpj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2yjrrsgnj.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ldkwplxn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2imbpixpe.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ustlpjkg.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2xrffnjwp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2dhlyusnq.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jfekaohg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ludxtiaq.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2qwqdgrxq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2whddbmdj.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rzmhdmrs.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ffidnckp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2irlojdcm.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2vhftrimd.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2pampyoyt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ycizhmvk.html


<!-- 参考信息 -->