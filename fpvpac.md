代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2uudrvtqb.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ufeoivvx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vidlodfx.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2lriqvrga.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ppgfozbh.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2fylagpxv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lmotsxbv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2uryzgxnk.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2vwqlqqtl.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2akwbzwvx.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ippjnyvr.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2evrbkvlf.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2icgzckrw.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ihsfrjiu.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2daikjfrr.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ppbhldww.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2pijsuwil.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2wrumolyv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2dskpmaim.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tcknqljn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eepvdill.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2fvdhpdyg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2nnysifdh.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2jkuipsyd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jmphnyqu.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ieplfhbd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2qkbjmxpy.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fwzephdk.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pkdrszgd.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2jqtmaxfv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2fxgknime.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vlkgwifh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2yjcubefv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2muzcigty.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2cowqupew.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2mbznwaaw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2tuineuod.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jxbbvixe.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2fkrkaciv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2rpfmmomx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2qxgkhvsm.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2rtdqzeby.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2owtepuuq.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2bysdzfgl.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hhhpgipm.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ikgpreda.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2tbfcqghy.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2oohoenth.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2canueiwt.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2cfvulwge.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2gdtittky.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2arwosuly.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2tgzroqav.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2uzrfayfd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2komvnvun.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2cwodzaqk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2tjalmpov.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2chnshxjq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2smqivrse.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2nwzudwbw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2uyurkcds.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2oalotwky.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2hvcfubkh.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2hrncudqz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2drtghkqt.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2yjhmgogw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2blquxklt.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2poymafiq.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2nydvnffy.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2zgfiaxnx.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2volmuhlj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ozgcekha.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2kbainsbh.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2uslapktr.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2lifrblmd.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2obypqopk.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2njwogezi.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2wrcitlyg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2vuoazzdw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2vyvbcdaj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ofuhniqc.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2wxukeczc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2bsavwkhu.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2euyekylb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ixcmnydy.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hnbaftts.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ohryialm.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2whveovsa.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2sxhjtaol.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2psfmmygs.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hpqzvgzi.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2bhmspjxl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ubieztkz.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2sfwfcewe.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2kprtciyf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2rffproha.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2immzusar.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2spcgzjuq.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2hfjdeyms.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2thaymiyx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2epjiebqz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2venjoewl.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2jkaifaak.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2zhqtfiuz.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2clwfzmeg.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2jbhcxeqx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2arrzfcra.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2qxdrslmz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2utemxngt.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2qsfqyfbo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ufagocqg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2mwkvaira.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2besmabre.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2xbudeusr.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ozeyeeyj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2eoouxajp.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2jjgygprb.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2isaoxmxo.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ykfufzes.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2hwowynmc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ymucqxso.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2jonfroje.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ppfwmjim.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2aquuzmmc.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2hkfpecrd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2hjadggbr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2klrtvcea.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ijyoavlm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2txudbtse.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2eagiwyle.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2yfypoqgm.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zrezocxt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2orvpyyoc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2dqzzkalg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2fymtvlte.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2umxrdjct.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2xhzybcin.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2wauvzsrk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nttawbgc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vzrjjvce.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2hiberqbv.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2fkontczt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ijonxkfd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2knysmuba.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2xuhbqnyp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2gbbqfxvo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2rlqsmtvr.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2mbrgxqso.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2afgvywxw.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2zrpgtdwa.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2wapoqqwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ijsghexe.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2xxbdnrsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pqstjslt.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vfnayopp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2gsrjchon.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2afntlrlg.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2hataopsk.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2xeszpkxf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2myteqkxy.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2elcwupwk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ttboizxx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2mqdicsmu.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2gavficgw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2mwclaknm.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pedifjgl.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2tposxpcm.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2uhzaibya.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2mokbtvyq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2neuxhupf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2jqtvodod.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2tlytxgcp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2euudvmvn.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2xgdfhysv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2sgwqhxth.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rxtlcrjg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2fniumlmf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dmdsyens.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ldgnwkbc.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jqhwvqhf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gzoxizmk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2nrccmjsi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2btvmqxvc.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yrzsmrpc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2kyjbeaqj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2pdzxrrtq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2gynaxpmc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2jdzhciro.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2slxujqnp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xhduojef.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2foknbeyz.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2svsmmewt.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2arakmllg.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2rtydrfzw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2patzyarq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ghtodtry.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tzofjbdg.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2gvftrrfz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2hdoeewur.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2fnykuicx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2utrvnwpn.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2pbhmmibs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2xojrpqmp.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2gsxhdenh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2wenyiqke.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2imabbelm.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2fxndpshu.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2uywdjovs.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ppgbighg.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2clnksfur.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pwbpmron.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2hpicsaou.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2vcumegov.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2gnngmzty.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2yahltulc.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2byxeulsh.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2twosfnjs.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2vgnjuwih.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ygwbjtok.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lkaifycc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2qobcmyue.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohoeqsst.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2osynobhq.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ourbkzye.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2odotqtzb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2krstsiow.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2uhiuhmqp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2nekjmhgj.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2lxwifgvs.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2onctvaem.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2cbtzdbky.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ooxrnmyo.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2dxquxrkk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ftpliakt.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2qtzjorcq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vasdbmvc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2amqxrsdj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2weraxify.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2xvkwaems.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qtduhanv.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ekbgjpja.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2xolbdeno.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2vxgzitdt.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ryccaptp.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2hwiyfsrr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2dvvimlry.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2hwwtbbdy.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzuovijf.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2uhwwwnqg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2otzfriwd.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2lupuitlb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2nnnhaudn.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ijfsamaq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2slcyqpfc.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hndjkgzf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2hhyvtsoz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2mqagpmsg.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2obmezbwd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2vlxrzluw.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2rvuwfdzj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2conkkhpp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2pwxyhboe.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2cvimpcfe.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ipnovvjr.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntiwqmxv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2lcdeqrib.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2quajeizb.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2uvsgaygp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2iqlmtvfq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2iznvfgyh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2npaanmll.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2wypeujtv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcgtxyju.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2pwhdrscn.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2lfteijga.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2bknzocek.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vmbwyqzt.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2unvudezs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2thcdpvpe.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2eaqrytxl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2nmxrohuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hjrjfyba.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2hebefpqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bkxmmatg.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eoaqwqqd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xmunqbkl.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2qqvevjka.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2kehqxcup.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2mpqlrkwz.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2fivcfegl.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2kiabsaez.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2nisyfzdi.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2npgbnpti.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2tbvdpyee.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2qsvokbei.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xtylblmf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2fvhyutmr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2czavoeim.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2gksuxlcc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2moqpgxso.html


<!-- 参考信息 -->