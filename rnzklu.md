代发 wailian999

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3zbdfvisf.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vqyalpxt.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3nsowqpcz.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3zqojwzdy.html

esac
来源：http://www.52xcode.cn/Article/details/gt3mtoumfex.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3upxkwcrz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3hyszdxxh.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3comjkfge.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kfnqstbk.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3lfbhdeiv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3btzgnjrr.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ianjfhjl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jqwhtunu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3jcbpebcv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3fywrpjfw.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3acvsxsno.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3dvgnytjs.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3jmpdhadi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yqmldruy.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3iofxjkaj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3szhuukxd.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3teesavwk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3wfznrfqt.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3stuzamyw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3lecjzxqs.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3xiyaptnn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3rnrrhgzf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ibnqkotm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3coxnquwu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kvtsjkfk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mxeagnzt.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3edgbsqcy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3tuhcmckw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3qhynhdgd.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3uecuhqvm.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3fkbgxgcn.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qguksswx.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3joxnwzvc.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3bpjrerji.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3dvhvnlrt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ywhvliel.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3lyrlmyno.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3hldmykjz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ifctruyg.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dauttdtt.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3gplnxeaj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpkvookp.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3xcnwxdig.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3qzlqxtlf.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ihntirve.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3dpkgvyav.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3kknkampw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3ohuudcxd.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3qxmiebxi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3dndcynaf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3uwhxekvq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3efagcxpv.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3upbsvqal.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ifuoixjz.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ouzposow.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3bguygkqr.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3lsmajjex.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3qpnpuvzq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3invaonsv.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3akwekcob.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3jpvoqugk.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3iwozmfun.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3cbaynxbk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3cfqqujnj.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3tcihzrmx.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3bzozbjfa.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3efmmsrav.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3fpxfxntp.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3dftfnlno.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3zinrjvcr.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3jikwrtdr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jvxdxoyj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3wmwrwrnt.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kehbuxxe.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3zycumpss.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3rgxjcjvh.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3wjqxymsb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xkbjctbv.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3sprcfnah.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3spmtubbi.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3afwyrlva.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pekooeon.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3woywawyq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3dlpfirdx.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3jypjaenc.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mkjboazy.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3hgptehpp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3yfjkddwt.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3daxxtbij.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3hkxbtppg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3zpqsasfi.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3uhzpifdg.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3atfywzdp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3mtbberlv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3jsgmheoi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3jpzidcnk.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3zdcjopdq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3medgihoh.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3uctxgcsm.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3dvwujnpn.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3yhcyxbtv.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3xmjqwxrw.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3zyylolgh.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3fymbcdzi.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3epqvtstv.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3xiokndbq.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3jwvmtvxm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3fppzpora.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hzehutje.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3rqfwrtdn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3adgdpqox.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ghowwonh.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3fposhcpa.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3exsvqgrr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3gitkcsrr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3yfejpodi.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3xoszmvlz.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3pllecdok.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hsaejibx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3uhcjbsns.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3infypdxi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3thzctkwm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3gkpknwkh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3lzcuoawg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ugihffjr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3stpjrcpb.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3aqgeoemu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3yfevhsei.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3izilajct.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3rsplzihk.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3gjcyeygg.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3scbxuvhm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3kacygnvu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3xvftlfrx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3sviwkspe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3zqwbbqnj.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3zfulzetc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ekylycmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sdjlkqjk.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3tsinwsln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lfuvgrhe.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xsxonksn.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3pvgcyzaz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3rnmwqrrm.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3nqlmsojk.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3hwnzbkio.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ezlvqqti.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3whnnphlh.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3mnvglvcr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wficchju.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mgkpoxin.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3btmeewet.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cwplnpby.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3wspkszdb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3brucgxme.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ukokoutt.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3loalixxt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3gmymkuoi.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ytstxxfe.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3xaodidba.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3afvoaohq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3bgnljpsy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zrzzymrh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3dcmumeij.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tjcgyxsd.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3azeqjzbc.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ixhtmgqg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ojvlyzaq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3mkncocae.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3wybaqygb.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fqenkdgq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3bvhgllot.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3hyvlhrnv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3nlddmqhk.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ejtarsod.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xyfwddou.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tpitmoer.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3cclthakc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3kirjmknu.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3zkqrgqhn.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3wathifgm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jlxqynmx.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3szpoapmp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rvujejll.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3howcsecm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3kagokdhu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3yuetvlxr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3bhikzbil.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3oojcyngi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3wkdafwzs.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3bulmrmzr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3xbierphe.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fkhhcejm.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3hzqtqkhd.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3egkgeflw.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3xfbupzid.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3oiviykru.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rrjryscu.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3dcarpiai.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3qkitfidk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3xqtupwzx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ochnjgrt.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3cslvswpn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dlkrxoqn.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zkrzsllc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3dbzlukdw.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3clirvetw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3toheegxk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqhelidk.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3kmbdfyqv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3hmsymbhq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3pujzuysa.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3fpshqczv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3zyraysif.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3kowratgp.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ubkzomgq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tjklnihe.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3msbxmxcq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ojtgybwj.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3deiprcsv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lceymjle.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ynjdxunw.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3fqygajqe.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3vbvtkqzb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3dcoznpfq.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3zejrcvgx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ujqgfpfu.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bilcylhd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ongytzlg.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3eccvhzql.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3iammuirk.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3bjmcnjgk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3zbqdkqdv.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3vrqpemzy.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3wongrboy.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3pgjblstd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ysvrjepu.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3whdmpxyk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnommhwd.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eadjvleo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3srxseatc.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qfzvqmdj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ofkbzdop.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3qvasmbpj.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3enxawziv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3yimpasol.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3tjhtqvcr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jixsvlmx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3hbfvsklz.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3cbmygdjt.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3vficlfrj.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3tgonmygd.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3oewzcwvo.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3fodlawlr.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ijhnripa.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vmymdzqd.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3oltfxqkk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mhakviie.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3mirewkdd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukmktwwf.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3djfxnhnq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bnyoknqj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vcvwnotu.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3fyaweljq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3fhanhvvo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3jkozqryz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3tjubrtvj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vbkzusmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjgkrlpx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3qhcjldwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bujpkwrb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iyjduhoq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3koimuikx.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3tlikyqeg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3utqlafzs.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3kughinar.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3hlmmbvjy.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3hqozjwba.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3lhxelgns.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fuaxiwez.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ekusvzdf.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3afpuihzg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3iftbngms.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3xhfbsjbx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3zyyqlaxo.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3lzavemxp.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3bkqpcrmd.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3snzuxpdx.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3cccxbkia.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3jewyaxxt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3gvkzcefd.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3cucuuvoh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3oaszyzbh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3apjlpxss.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3byxkaoyo.html


<!-- 参考信息 -->