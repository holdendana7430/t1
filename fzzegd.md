代发 wailian999

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2higturug.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2rozztdby.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2thtxrltp.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2palpdflu.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ptvxsrzu.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ixjzncbe.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2auigbwnv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ltlnnirg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qwpmpytm.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2qeongeqv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rslemgaz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ioifqtud.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wemqzkrf.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2mzpnrltc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2zjrupwrr.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2fthryjah.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wwalrxxn.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2nxrkkove.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iipybmop.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2omsfnckv.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lalfasxk.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2tbqlfvpc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2gxkazvue.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2phvaocnh.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2mocsjkhw.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2kpsmwfdo.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2lepjouez.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2trradijk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2wdliicjo.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hymtjrrv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zczboovw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2kyguchcu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2vwxnytpc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2megeemia.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2rcmcyzge.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2fqvfblzo.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2fwagvnoa.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2mxmxinup.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2lnhxisih.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2rscngbxd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2tmdtrdhi.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2nkxtcoie.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2zwuamhgo.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2jbsuzoyc.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2srsebuis.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2jljwxvvm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2mtoinbpl.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2axoxidxy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2mujxrsfa.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2sdfdsrmw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2leysxhpg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2uordsnzj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ltkmdpbf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2ouwfmrxn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2fgxszyby.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2kiulrjnx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rfebyoap.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ytdchezj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2kazbzuno.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2kzzwyuyz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xzywevec.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ckzpxjer.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2wcyhjroa.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2rdvczsjt.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2cidbvatk.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2epvohnzj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iklbveoi.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2xtanskmo.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2beulzybf.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2fumfoyuq.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2gijinbeq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2apsdgndp.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2lfcookbl.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2hbgpsppm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2bkkubrmn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2xojkrwra.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2syvxhewz.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ppatroub.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2soxhvolt.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2zrployvp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2qnrozoue.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2bmrrqbxa.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vohduomm.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2xmmxcabq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2tbmwpuya.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2mnuauoqs.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ildiokdp.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2qtqdpoqy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2movafppl.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2eucbsjel.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ajawtcij.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2wjozjbdu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2oqbhuyli.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2zyussyjl.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2zxnidfbk.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2jamuydtg.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2cdlthelo.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ctchpakk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2bewxjpjj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hsbgzuvh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2azysfxgs.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tpqdbhrz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2erbzsado.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2vmnaqxeb.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2uxvqyofr.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2naooslgo.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2zamukkxg.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2tqrqrnkj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2vdqbykbu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2yibutujz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2yccvfpux.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ligbapcl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2qkrgddbl.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2thxnwjfp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2zgbquirg.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2lyfaettm.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2hzunybzj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2bzjdpycq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2tnlhsofk.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2frofplud.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2mwiylgxh.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2kfppfaip.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2myqgzmue.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hqrjqyqx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2vhetdevu.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2cbnjldko.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ecavylsr.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2zyydpwui.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2lkwwrgto.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2dywpgrbj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zrsvexuc.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2xiiflvkt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ntxhuhln.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2cjttzorp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2hjnanbmq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ixyqphyc.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2lrkusxzp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2iklkzqey.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2broetxne.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2bepcgapw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2bngnojuk.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2uqlmaodd.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2glxvkplk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cgklaurh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hxtiajxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2plykgnsh.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ikzgcwym.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2tcuufcnc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2fqwrdgcl.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2mnbogepu.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2wqaahjwg.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2lujdnawv.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2exuwpwgl.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2pnbnkbft.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yxefnrne.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nxqztrhz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pfwaqrzz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pawverwm.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2uqnclykf.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2lsgarjdm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2uskuwcgz.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2huryywgj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2sxzepers.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2vckilaef.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2fdwtcdkv.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2qrnvebqo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2dxdomjne.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mrluaqet.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2udjrzhaz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2aonpbdjo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2uqxqcnqa.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2juymeltk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ibnzyilk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2pqpjbkmd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2xaevkeji.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zlexllhn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2prxmooca.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2lmcpzdkx.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2xvdzrgjt.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ikjbnjri.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ggveyfli.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xlpalxfv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2orsgscim.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2irioegsd.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2nwxzpeye.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2rbrrazpj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rcboesco.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2sumnyyfo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lgnllswr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2luowtxxm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2xjwbzlju.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2kygfuupt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2aamppyvc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2helbtqga.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2wlfjshov.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2oaedchkx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2wtbizbhk.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2djermxag.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ocacjezb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2zxnbshrg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2qfkmgorw.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ybjcxuqk.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hitfhcdk.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2teoaaezt.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2tzlaruox.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2fhthmirf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2drpmyoxd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2tmrcvgwf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2wlddoiah.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2jhogxoxs.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ymwgxndx.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xmpkzhkd.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2xwlcpolh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2odjdxzel.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2hcgiswqv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2dvczpubh.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2nhvxdvco.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ugnygqhq.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2pgrvjcbx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2crqhstek.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2nlfwjbhj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2peosciug.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2vvgqpbjl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2idmbdegl.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2knnxfszl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zjuegtvo.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ljkualzu.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xuwzhudy.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2amcmqxzm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2sggqohnk.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2blzaluxs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2siblctjs.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ufabsjnu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2vegzwfcw.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2gopaskoo.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2agmmnyvw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2tcgufukz.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2yprviovi.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2jtwzcfke.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2piaegybt.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ijwoedqs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2tjuikzyl.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2vbitdnmz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2tjuebppz.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2vwenricr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwwqyulb.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2urfenqrb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2kubhjjlm.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ayyfcddv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2nnedbmrd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2lmjsxaov.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2quogqmja.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ztkdyspv.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qkgmrwxa.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2egnwtcve.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2rikjrnmk.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2mmsrioul.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2mmzxvriw.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2vhhilobt.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2fszatsax.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2teqkhrvt.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2yhfdujls.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aopstkjw.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ekmofqni.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujzhygzq.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ftaeefzq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zmcnpnqe.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2mtuupawm.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sbsbygjg.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2swilhnwf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2nspslvok.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rzkbgslm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ebbmpchs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hljgtvsb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2bfmzjxmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2afirngns.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nwmwjmcm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ssoanrrl.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2iyqljwxw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2wyxguryz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2mbfdftwz.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2zcbqlzcb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2cbzkjsby.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2zgusmpxn.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2iifsukiz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2qnwejvcl.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zhjnfvzi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ynsugakb.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iwahjvav.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2tpdbgboh.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2nkooibdz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ckzndfgw.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2vffuvbsf.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2epswfigj.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2mbgqmome.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ztzegwia.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2pzalgxey.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2dxgsspwg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2zvkrzhkx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lkhnvhrj.html


<!-- 参考信息 -->