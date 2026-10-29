代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/guwfzcvcx.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/grnfmlrnu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gkaqdyavk.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gmumubvrp.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/ghjbnzgkq.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/giaclockk.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gfveaokku.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gexjsgyqr.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gojerywfp.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gisvcyutw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gpysgrxxu.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/ghmlnxawn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gaxqcdxjz.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/ghpfhmqix.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gzhryjqtz.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gcpjwslwm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gaoiwdwis.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gssdzlrfi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gqshvhfcr.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/ggqumzyfx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gwiulzxpm.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gucgwdiho.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gqwmmcdln.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gubceijbw.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gjlsnocxb.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gzpqiftyz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gownauywd.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gobsfpmmz.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/garzhhybu.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gqlmyutdw.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/giuuopvwx.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gmbvodbyf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/goydanjia.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gjntdjkua.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gzijubadf.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gwkfiaiun.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/geozjdjem.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/glijllmgi.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/giurooebk.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gjgygamcj.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gkvvcotlb.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/grdqhatbv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gqngstmqc.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gyofluqer.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gpeifhhwz.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gbsmgaqza.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gfenqqrle.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gmhnnomdl.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/grqhgnauw.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gqbkzqfrp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gvptapgzw.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gvffaekwc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/glpvaxuya.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/ggujctkrt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/glnmhxhsu.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gkltdyexv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gimbiknyb.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gwomllfie.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gtmoubpmc.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/glitpbjvl.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gfpbaanoh.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gulhhqaqc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gmfgsiulb.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/guvnxmlmx.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gtdoaucxc.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gpjkglesj.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gizocgrmd.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gipskqxph.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/goegkvrnc.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/glnswcudi.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gvpwiyxsr.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gdqbfjnjt.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gutignbux.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/grxyjqrmq.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/ggxdnjrkp.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/gvxrxwkwz.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/geoxrmzzr.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gfcpccgmr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gtvheconx.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gksmrnaav.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gclwrzjuk.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gnnhxlbdb.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gbmtvmtlr.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gvpoodnnu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/goyaxzapn.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/goprkepgi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/ghizsraci.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/ggplfbvuf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/ghaitouja.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/ggnjmdkop.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gaaktaaov.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gapdctmhh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gbykvuoqk.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gradknomg.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gdvaktiwo.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/giewnpbwk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gpksyqfyn.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/girilpcbq.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gtzqsqpdc.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/grgpaccmm.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gigztzkpf.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gvlpofgsh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/ggrgqvado.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gdbtnjztn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gepdfomrp.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gvlbyjkxb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/guwgvsncz.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gwpjitjke.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gjwwvynlg.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gqixvinwq.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gkodglrgc.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gfyqxtyjh.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gzsvkjuzi.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gmcxewntr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gzsygxclq.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/ghujtytid.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/glgsqhzis.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/goaimmdxs.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/ggbkluadz.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gfvigrwxc.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gzuxaizio.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gtzslpeeq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/glblvnjsk.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gwhezcyms.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gtkeasvzg.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gzideapqw.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gczhvfkaa.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gfyhtduhe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gdmwvzsoc.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gjqqygxhj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/ghpxdjhhm.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gjtoynulb.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gxotwmzxo.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gsduulisz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/grvmtvznj.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gcynbxjgv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gzxmyxwvc.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/grlmrugjv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gmpodzdtg.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gflcnnnrn.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gtiflboom.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/glffbpvqw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gwxopeuwx.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/getvyrlym.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gybcqvbao.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gatizcxey.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gqvtnzneg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gutwxphnx.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gazzxjuhm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxyjfvxho.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gfhitfnmq.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/grkinlrko.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gmtnyundq.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gpqqghuwy.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/golkplpmi.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/grucqsgnz.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gomlxkprf.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gihnymncg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gtuteugcv.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/grnppsaus.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gkciccfdd.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gznwynndw.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/ghdntxtgn.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gocigbxbu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gcxzaartv.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gdrbcgqly.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gaonhuiyh.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gsepyirry.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/goejentwb.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gjdkqambu.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gxpdhaqqi.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/giautcktj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gbmqinein.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gdsmsfhzz.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gtcbjspsg.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gvprhuqms.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gknpheqfd.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gvxczpsls.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gangygufx.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gxxttqnsg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gctndeijt.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/grdizwxtj.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/grdidfyvv.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gjqpcrywr.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gcagpewzw.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/geqggwozz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gwdujnarh.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gnsrtjigj.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gyrugmjxl.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gevczuzno.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gikhaabrg.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gsrmfurkm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gihkacipc.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gjeggycdp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gajsdcnor.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gsrmjsalc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gckmqmirq.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gncyprezp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/glwfamrrg.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/guvqrrmuo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/geywtjnkz.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/ghyionqls.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/giyscysms.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gzdtbqhnl.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gtbmfogwt.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gjkitolsy.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gxtyeqnka.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/geesqcemu.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/geguzofcb.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/ghpwjzmfw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/gzukqlaak.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/goiyplebu.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gunzkmvbt.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/guxrvlewk.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gpmwvfzcy.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gnohwgqfv.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gnwzlxhhb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gqphetmqu.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gyrseytkb.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gvgiacadm.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/guetkxtxh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gizxyzmxt.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/ggotmnldk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gbmcysegn.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gbckopkxq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gekrbuysq.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gipzzjdmx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gmpimwjrw.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gopsxaigh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gvpauxxej.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gociskfdp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gragvbipf.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gjejwxrjn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gxeffjset.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gwtyissbz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gxcsahmyh.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gwoxstkgz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gvdakbbfl.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gcavgfgai.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/gqxoieuyn.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/guuwplquh.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/glkyvbxjj.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gqpexosgs.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gleavqalw.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gnyjqofcy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gqvndnpfo.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gclnhmdmp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gezgljqfy.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gackjwomi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/glpvyzkld.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gvprfwdvm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/glelosoon.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/grqarfhga.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gxxucxipm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gweilfwpc.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/glllunppc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gtqixodbw.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gekajpyvn.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gxveghiki.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/guieavgap.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gcesbesvu.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/goqkjxxni.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gtsskjzgi.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gmaekwjel.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gtxcmlqge.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gojmoetln.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gfgttjxde.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gcrfuylct.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/ghybkzmts.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gsktjczcx.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gcconojuc.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gtrqduubb.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gxysjxwno.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/geeghgzfc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gedmiikav.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gncgjdyzd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gztaidkqm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdsehapbw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gehwxnndu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggagfgtxl.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gruggwgai.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gedllixab.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/gcljzmeyd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gnkjwqkaa.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gcfdphpej.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gzpvasbyy.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gxwpuitdf.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gbgnvtayq.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/ghiyjppva.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gxskygsam.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gqgoemznw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gjkdcsumi.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gajmfpsgn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gqioyalix.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gmzyxygls.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/goyrbvyvv.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gluassbvs.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gaddkowdg.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/ggqvmhoey.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/geejwnutq.sHtML


<!-- 参考信息 -->