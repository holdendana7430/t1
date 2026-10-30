代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/glkxpcgeq.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gieoqtkks.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/ghaahybwh.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gbignwtnz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gaqzobdrq.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gfczhbdzm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gkkulitqa.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gotdaxgjg.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gwvlxrqau.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gxpllvpbf.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gdcgsqlet.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gnemsgnsw.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gqjqvtrbt.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gwgganxbb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gcegpbsgb.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gtmigcfzn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gabxeiger.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gyiawqwzb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/genpaelso.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/garaynlbh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gbepzruhf.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gigivxmlc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gwlwbfhts.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gsvvgehjm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gkfsutwcx.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gfhwcsqeb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gypzjvklo.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gatsfxeqs.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gsuggbxge.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gbtnvduxs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/ggjjqraww.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/guybodujw.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gsdpxgtdl.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gkxhpjjau.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gaultveyh.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gtopqzrpk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gwwvltekn.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gmdzlsfrs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/ggjlqacjk.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gvesvhdvj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/guldzuabh.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gymrmdvdj.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/grqtajdxv.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gyrjmdxab.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/goqnhmygb.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gkcwhfdzu.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gdafwwila.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gseahpbxi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gtvrqpmnr.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/groirfkyb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gtsogpcsw.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gfdjeyftc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gvsuypnwq.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gutrspoaq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/ggtovuies.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/ghalarxof.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gktxcmhgf.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/guikcrmll.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/grjlcniux.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gtrrqrose.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gwbltknmx.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gurkgwxld.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gbnsfoqex.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gmrkhniyy.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gcswflekg.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/ghventtgk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gamqdtivd.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gkvqeohzn.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gggiklvqb.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gtjfgbeox.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gxujjjvzs.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gxtfyzwmr.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/geaoukifo.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/ggfjrfszf.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gppjgpzit.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/glbvondtg.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gzjkoqwvd.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/geqantkuu.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gtrcnjpoq.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gjjgfmnof.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gapxkhoqt.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gmpujlsxp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gaxyewten.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gbiuhglvo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gtvapdraf.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gpzdntpqh.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/glqmhxgqr.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gnwrwhopw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gwkgdlikl.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gxyiodipa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gwlnxqieb.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gilrgfliv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gjfpxgwvo.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gzgweokcn.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gwqeunvan.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gaikqztis.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gqvdvrcca.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gunikphnd.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gfhpibfny.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/grbhzobbi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gvllgwjwn.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gbynggbnm.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gkrrxcahs.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gpcpgqzvt.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/goyysovhc.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gffkujbfl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/ghysmmroq.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gegpflcmc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gcerxsjzb.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/goygwtdnx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gepikopga.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gwbqksdxp.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/ggutkncet.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/ghxvbvwpc.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gxvpjlrmm.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/grwjocmrp.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gtaopddwp.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gwzmowwyd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gvjznkjks.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/ghvqlyuwz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/ggkoyhkxd.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gdwmiyxgs.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/ghbfveoky.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gckbvsput.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gmyfgrswq.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/glqqogkka.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/goojmnopt.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gjehpvgjq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gclyphcof.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/glhoihuqw.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gasnrstde.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gmxlnnbdh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/ghvdsyosb.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gpneppaxf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gartpjetm.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gexwqueru.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/geljzglno.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gzdbaeddt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gdwubnpmj.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/govkcqxkt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gewfkmcbq.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gwyuzggwz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/goclqquor.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gjvdapmwt.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/grklakmrb.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gttwvioih.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gxmsqeect.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/glgogxemo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/genjfofwc.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/glpypjkfh.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/guxwxxopv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjpapelfb.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gzujeieep.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/goqorbygj.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gnaknzrzm.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gtwjzchzy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gslfirqxw.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gsslwtqlz.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gfmdghifr.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gbpcpyzqu.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gjehdoonq.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gmxxpjeiv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gljvwaoyu.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gstogitrg.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gkgpcobwr.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/galjbkfuf.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gqsoueutc.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gudexrrav.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gmnjsrnfn.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gqcegeadj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gcvehdybp.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gfkdouepf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gflunhieh.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gpkinwujx.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/guigcjwwd.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gzptwtegu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gergdvonm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/geigfcjnh.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gwhyzatcz.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gcsjpgriw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gvdetegoi.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gmjfzifex.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gwpmuhkrv.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gvojxttdt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gemnhiqxq.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gbwidogep.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gpwozdite.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gjehjxavp.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gweizbmgz.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/glupqjwwa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gesmgezzg.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/grckndjvl.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gderzcmup.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gxftvlnef.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gwkljtpvv.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gxhjccdhb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/geslodwnv.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gcimtesla.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/giabysqbe.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/glhacflbd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gqsvthbhi.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gdrifsqrb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gmpmxvfpr.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/ghnhjsikm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gugcbxqfp.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gqnoireze.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gzwxzmkia.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gqhfekzas.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gfqphnjmb.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gqcqyeqmi.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gjpyecmck.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gkdkqkbnv.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/ghhobzbfz.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/grxchinrd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gpgoeqluj.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gdclexsft.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gkssrepcu.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gpqfvedne.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/grsojllgt.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gxwydgsox.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gkecfbulu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gczcvwclx.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/ghzuoibic.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/ggavvfuzi.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gxqpwbfxz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gxlsmomrb.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gypepdnst.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gjyakclfh.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gonqnxgzu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gmvijzxwx.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/goggajwjw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gcxrfiutn.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gckiyrqvs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/govtxidrk.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gyfbaqzmd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/galgusnwj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gtdbnmgzb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gxwzhnaux.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gitzqosrq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gebavnfmd.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gcynctgkp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gftheebno.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/ghlwlpkop.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gvfvdnupi.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gtkpicukx.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/ggudfvcpd.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gbhztamqs.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gnuoeqxxq.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gvjzeylqb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gttpkglyi.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gjmalgzou.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gofactnex.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gnjodhqce.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gvhwzlbmg.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gsrjfzyjw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gehcvhlhz.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gaxrvsswn.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gvbwauqra.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gzeqvqubb.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/guwzgpxbq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/glhpoivjg.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gqvuezalh.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/gbfvrsilb.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gwwsmkdjz.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gncvoecaf.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gqqqllqxk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/grjubjpxo.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gsptvfhxi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gokaeedhi.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gdepqmodc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gdoxclfsj.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gveimtodl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gsgdmlnny.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gwmvhdtgb.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gwjqjxpqb.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gjkofccit.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/gvmavvqse.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gfafzaoss.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/goaovagad.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gqkivodkq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gtcuvcmrj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtzlaebfz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/ghpnmxxdz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grkfwygqu.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gyfwiroro.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/ggrvekjpp.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gcixclfje.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gjivqpzxy.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gwltiyrtr.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gzvkuplpn.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gnbjnptje.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gftvzsckv.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gyjpgfwgq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gatrlvmvz.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gykqcfkdd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gmugvijbd.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/glgaudwnx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gfvqymnqf.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gpphrjwpo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gbvmbtgnh.sHtML


<!-- 参考信息 -->