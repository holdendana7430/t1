代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2oqaeoepo.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2wvknrxvb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ejkfldtw.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tmxrgftp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2dvsolbfh.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2xkvyqsfp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pfyxefkw.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2miklogks.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2xouwkhgi.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ctiyidto.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2azxtxlhg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2nqxsqpkl.html

esac
来源：http://www.52xcode.cn/Article/details/gt2bsqxgyci.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2yszmptdi.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iklghhfg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2isuryorv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2pxowrmeb.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2hfgyoyzh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2urbxlhnr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zbrqtmiu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ryasijdk.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2raatfcpc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2kcofwnwe.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2winjoadh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hamgecec.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2tqzbpqvs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2zwhrtubk.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2alyjiate.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2jnhlvzyh.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2qwubdddu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vagdsqua.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dquhunsm.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2iogvcpdl.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2fswcnlzb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2htuwudip.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2bgdpdzhi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2eypawlqj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2daeidjbu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2cwnaggwr.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2pboxapgx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2uaefjlzu.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2nuwuvasj.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2stbdqcpx.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2iwpsplym.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2mfzofpxs.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2eyxfgktv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2qlrlkusu.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2lasxsuzi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2iijlobjz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lbuovawg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2cuxglljk.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2cwtqdkcj.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zggjivcl.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2teewrpgb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2edmsympc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ghfoprvt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2tqkpznbi.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2mvoitmmq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ddalxlns.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2xvnzdjqv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2nhzbrjpe.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2hekgruvw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2cbhhspmj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2xmezinhz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2tocwdxbz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2rsmmwrzm.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2wgsghobp.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2lyjpqaxc.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wrwyfhho.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2zhpbpbmq.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2uymtyfma.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2epfshinq.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2eqtsnnhy.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2sgoxecvm.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2okqozjpb.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2pdrvtlpi.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2oagcavmf.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2hvizhgjx.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ixcyypgl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2njevbjxe.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2pwyxtwxh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2yiwkpplq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2tdsficsa.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2mkirttez.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cdoglgtj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2jalhacns.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rvpgdxef.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2vrdjqfat.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2jokvvzdo.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2eikhdkbk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jmxsunds.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2woxqyaie.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2vgxmqwlf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2blhdysjv.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2akpsqzqe.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2dycxgjvp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2xpkjdgpw.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2uayapmmu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2roqxlumn.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2truvqzet.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2odmyhhcs.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2arqmnrxh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2hhajuugs.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2hclajynd.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2dqlxeudr.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2iloodckv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2hlumbbzi.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wztjlmge.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2dhskvxlx.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mirwxmbb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ndrbpmgd.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2yqqpcqfl.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2hvsdajgw.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ayjuyftl.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ubszkqyc.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2qajbkrxw.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2leldahil.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ejqdkyfy.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2mkvkgxze.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2gwxexsvr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2awhwjxqu.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2fdgvzbae.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2dmbjabvo.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2oagxhpts.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2zuojzxvj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2aalhdewz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cgueicjn.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2suldckyr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2jwcjkyfk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2ppxbrlzq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2guscgzgb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qclkubbh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2omplqsmc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ezkeyikf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2impkuskh.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ziycoenq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2zdoqiuip.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2dgbrtgxp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2srtpeelo.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2cmijpqey.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2joeqzent.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2isnoajop.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2pmqmgmza.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2nzxobhyh.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2rnwbbnoa.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2vztruqbc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2smersbab.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ogcshwtv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2lojqrzgu.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2hkktpvvc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2eugvlxbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vfzsikeg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ypflekzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dnvmwmba.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xmezrotb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2zivjksbs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2nbhbgupx.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2aeuywyyt.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2rhuszjcw.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2zguteifr.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2krgwghqa.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2zhdxdzaz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2hkybsiio.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hbdoxzrk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2dlanpwsu.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jcawdszw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2zkvbkyav.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2tywckmdv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2tqivdaas.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2zcqhvarq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ysiteavk.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2aafvpmmu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2xkxvymmm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2capjqriv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2avdgzqpo.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ssaiycui.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2nvuzbnqy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mwurffjh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fovvscfk.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2qqkppkwy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2fulwttcg.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2obwvkjiy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2vroecetx.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2urjsuvim.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2bwquupfl.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2vdwhzadd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2xhavtyya.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2zbwrsdvd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2swogwidc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xamnuohj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2rectgrnf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2muzhyjgl.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ectdkyjx.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2vxamezds.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xftodsqd.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2edqilxnx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ojcatavb.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2wodovyum.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2rvkntols.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2bezrhkfw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2beblxnhc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2cwgxegkm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2cltdfont.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ajbaqfde.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2kfhxrsuo.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ynfgqzyf.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2kemeowwj.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2wztyukyz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2yruadbuv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2gtaghmle.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xinyaijk.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2hubmvkyw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2hqpyynpk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2gurboiyg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2goydgcfs.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2qfstmibq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wimkjkvo.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2fzyyelbu.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2wplrbyar.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uuqdfswe.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2spefzmjb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikdeznft.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2oarugtmd.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2soatpcpv.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2whvpsdes.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2fngxfelv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ygsmehkc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezrooboe.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2wiypgqqm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hgpprdxf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2taaeenrc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yqldbnpu.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2szbhjxkr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xkeacqpv.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2rmyjkocw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2btbqwbxq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2kgtlmldk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2zvzweuvx.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2wqikjees.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2gkkmxegw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wcqkzzld.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2zhptkkpp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2qyxupcds.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2hqchkowi.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2sezaqwff.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ruodeges.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2lmpqvnca.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ilaiauvd.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2opyugnjo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2atdywmom.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2digekkpd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzxeqbzn.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kqeijuyc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2kkzcccuu.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tgswjmoe.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2fayhjpph.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2zlccqcok.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2aeglimfj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2skclkipt.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2hljkbxvy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wisvvndo.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2nyuffsik.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2cejnhfby.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ovxdovnl.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssuslhhy.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2lbqqzhry.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2pkhqeeqd.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2dqsvfkld.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2uduafntm.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2cpglgcnx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ombgyvnx.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2smxexsyc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2zdovllrp.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2jixeqeqd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2rigxlxkk.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2kvpwblwh.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2popciwgw.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2moypcqcc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2mcvdsrjo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mynvojtv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ygrlmgsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qjdyofdc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2fjxzrmnq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ywrvcjwq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pjhgbenr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nsvpdnoo.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2tsgezfwp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2sdwapbfk.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2fsohqzit.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2mkjrxywi.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2fquohwjg.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2jvoamabe.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2zmmfvfyd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2jaxyunaf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rpvtwgqa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pxryndra.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gefxbfry.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2bbjqhdym.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2rvecxbxi.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2lemnxhzj.html


<!-- 参考信息 -->