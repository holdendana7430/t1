代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ntavnusy.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3plbdhozj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3fgxxtuvv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3zxaqhftn.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3flnaexty.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3fsnfhjjs.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tdiurkid.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cpamnwpu.html

esac
来源：http://www.52xcode.cn/Article/details/gt3bukamckk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3qkzlbghs.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ewfkvdhi.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ikfzhsfw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kqvghdip.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3lrmpszqs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3frhddhcy.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gmnqccco.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3eexiijyv.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3snsefapy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vsxnwppr.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3vtkqyszy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3tycwogjq.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3iqbbjcqv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3knlzinsr.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dzzpkxbj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3rukihsia.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ywuscbft.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3jmosnbdj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ukdqhyts.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3fuxqilfv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jocipxqk.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3niffgaxp.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3mnifijrs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ziqfyimz.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vrqyswiu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3quggwwbj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3jiwdblga.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3lfwcxgcz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3uyaatffo.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ohymatsi.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3igsiucjw.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3oqwtemrx.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3yjsoasxm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3fxvselne.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3dttdqtoj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3youerksg.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wwmbqish.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3kebaopxd.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3otxxbays.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihwvbuhm.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3tkbokzrd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3oqfdoquv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3bmmegqda.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3zuvokbiy.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ajvacdtg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3btfdczid.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3kqtsblfn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3wvypwhmk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3cmuryjja.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3trxqixtb.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3xdqldzxz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ggmqtqop.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3zuwynpdr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3rqdmpmym.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3zocmchpj.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jxnksxvy.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3nkqkkjsi.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3hgufdgmb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3bvumackg.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3dmpfffnw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3qcfuleof.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ubthkmpq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3duutsvic.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mrftedaj.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3bqtpvfce.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3omvcmaad.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3zyhjoefe.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3frmmhmog.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3dqmlztic.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3shikvqfn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ghzaeifx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bpitabvp.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ofntsrnn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lkoubyuv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3dhyvajdo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3snaimkwq.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3dcsspxhz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3maedfxkp.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3bnwvqwtb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3glfavikv.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3wovjbgbw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3roqfqeak.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3vwxhitsl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3lqcehotf.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3zsvrynjp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jjzkxmlj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3eejffvdf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3vntdfvkz.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3pvowaevd.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3zvrpwvic.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3jjuiwfhw.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3kmpnmftt.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3gcrdsjhq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ldyaooox.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3aycdwznv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ufkbukhr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hhhfatfo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3iqqwfnap.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3nprsaqdj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3rbprgpwt.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3tiypgxwg.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3xplrvzxm.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3opvdbnpj.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3xmtshyer.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3pmomwaww.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3pcmmcull.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3yahvjptt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3bzcndhkk.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3wuhcxxlu.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3puztuujo.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ccxdlxzv.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3dexwzrks.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3kmorseiz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3fpfacjep.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3qnjgtigt.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3jqfcbfew.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ukfnccce.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3gwybqjot.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zczxpwzr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3gcydshqs.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3htovfncg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3rtyrkxro.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3dwpuqprw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3aagpvnmp.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3zswkcmeg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xpmwjrol.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fvqhuhke.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ftypkdqa.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3rcrsssbd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3lhkgivka.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ryvbdgbs.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3oqtvhpfe.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3apkdudvt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3sekfafbv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3dhiavggv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3qdyqasug.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3dsyhicsr.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3vcxfecbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3moianmtr.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ernmuvou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ixvasvit.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rbtzldqm.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3seerfmxe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3qowybayl.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3wnyoguvw.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3mlitzrck.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3tmvzizda.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3dftebccf.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3hbvsifih.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3szpgqkzn.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3exrinuxs.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yhqcglmb.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vxgpwmbm.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3zxuxmhqe.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3niiesvpu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3rhuvsohk.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3orfsfwze.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3owkcixwj.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3mtidtgzy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3zregpkdw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3jvmuhvgw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3nlzamqhj.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3llfjfgcf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3vwdulkfz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dxgjosfi.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3buehmtvy.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3kltivgbs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3wftilcps.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ydvipunk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3pqtxzwra.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mionnovd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ibnewrgw.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fhmgcoth.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3glilszsv.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3sozbwegh.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3srnyvydo.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cdsoepdz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3hnkumges.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3neqveuel.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3zqeawlwo.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3fsrixsym.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3kzdtqevs.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3uqzytmgq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qxdgyojn.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3edvykeph.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3qnttyvje.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3alaszplm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3cbgeripa.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3gusxcjus.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3gqldghzw.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3jxqhnoqc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ywsrpvvf.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vaywuuyg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3aasgxrir.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3wwlxfhoo.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3azhwzncb.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3vinnvcff.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qjdaafax.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3qnyispfy.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3bnonaoya.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3fjjpghcp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3gdvifzva.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3vhmdxggp.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rvwsxwvw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ewpygxkt.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3ueravohr.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gmoeoqzl.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3nmbobnxl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3fnfwdfgn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3cuxiaicz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3jczfdcod.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ilwsxqtv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fdxkubho.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3bdqpwowe.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ptlnpwno.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3hjliaatf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3oxvxsmkn.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3nfrhywuh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fotvutwp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3hwojdrky.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3basvkyic.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3lyvdyqlb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qbpzsjwq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3exoqvzjs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3kjgjxetv.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3soplqijw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wurcetes.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3vwwrdocr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ssugzesf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3lfuszueg.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3bbnudrzs.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3oiwxiiva.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ggqkhxnp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3zycfboyq.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxyspugk.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ouzzodep.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ywhxubmj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ckweteep.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxbaqlea.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3saacebtg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikqpandx.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pjexenql.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3wxnjjshs.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sncaopww.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3meubosro.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3suqjoazz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3vduciijm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3anhikamd.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3vqumggzy.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3goydawov.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3gshwkbcr.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilmrinla.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3exkzahrt.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3xzhgzghn.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ovaadfls.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3laabfylx.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qsbceysd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ninddccy.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3zakcfxts.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxfxzzsv.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3dbajxuvz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3wbtpfqca.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3tupiiqhx.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3qthlugve.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3dwbhzhrm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3hzixgqyh.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3fgvdpbna.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3pikpwqvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lblmyvoj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3umppbfuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwumkkjr.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3othcpurn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yjwazaag.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3fxufbkkc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3hbgboxhz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3vndeaghh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3venfwyll.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3vsdemoui.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3rjjxyjmr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3adzpoydy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3kgvtiviv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3eovdglhs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pyyszvrg.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3qqpysldt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jpqnjnkc.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hteicsow.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3obgjzgqe.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3fjjcjteg.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3pzjpfqdb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3jucyqanj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3flgokdeh.html


<!-- 参考信息 -->