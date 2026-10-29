代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gchilvxmj.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gcmfjbfos.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gjljjzmop.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gyrjkuaou.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/grayncnpc.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gfojmmhkk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gcpyjgbnd.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gvveduoyk.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gojtijmam.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/glenledty.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gmgpektcp.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gchmzuevp.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gcyblhzfc.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gujepnagt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gxvivzzsh.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/ggrdewwnt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gcykfketx.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/ghfasesgt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gkejbibjr.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gltiwhirw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/glrwwoedw.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/ghtsekbxv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gkwrdzova.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/goxxrsobj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gcdjjqnqw.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gseuewjuj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gobbykrbz.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gcgycbmwx.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gtafczarp.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/gtmmnschn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gmtyheamr.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/ghhlyvnml.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/glpowadtv.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/griksufth.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gymaornmg.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gufhfrasi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gdxfuipnq.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gzszjlqzk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gxulwehej.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gsnnatxjn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gikydoktc.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gwnzgasdm.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/guiijdzex.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gbbplwojh.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/givzqsctr.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gjzgpkzjw.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gqfoewsdo.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gjhtwjpoj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gkipjaxui.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gtoeejxia.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gslycvgns.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/ghlbovojm.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gkoatkbye.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gcnojpbmb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gfhlodtio.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/glszcrabf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/ggkosatbc.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gvpspvkpe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gfkcuhqlz.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gixvduefs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gzuluzgfh.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gikkpiwmq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gxtqcgwoo.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gfepnznwu.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/ggageqkol.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gkvefpsoj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/grgqrjbki.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gqkjyzvyy.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gnoogrzmi.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gaapndhfo.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gdincicct.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/glihwmylc.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/ghskqojqe.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gaounzmjc.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gyrcwiela.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gbjpoewua.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/ghzmdjbyk.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gbpkxoxib.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/guvgrwjyz.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gxwmjlcrp.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gojovfsmb.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/grrcxytzl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gukebnyrx.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gmqfjjsvo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gpcofafil.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gjldymdms.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/guqeehnav.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gicrufbwm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gqytvehac.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gcqbcvkgu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gpehykdkz.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/ggfikqyur.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gpphuphau.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gjdukdpyu.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gmnsbmamm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gnjzohvnb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/ggreytpoj.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/geposmnqu.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/gdbxsdfvg.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/guwlbenzr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/gdjglvjvu.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gxlpqlrpu.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/goymotsth.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/ghnxbayyr.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/ghdzacrvu.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/ggcznsayl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/giyacnvud.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gvwkovbxo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gjstfjiod.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gtkqjxjvp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/grjtarzav.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/grcuwtqno.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gcnzpcvvm.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gjmdhtere.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/ghpzxhhlo.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gzkbugzcm.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gwcudsdgl.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gjyerqgom.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/ghlzvxynz.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gzyejsigy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gfgkzdekf.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gqoxwfqid.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gsxeasdwa.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/ghbyasflg.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gfhcsbzmu.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gefjehnfz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gohjshmdw.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gscknvygx.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/ggrdaijwp.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gcrwktaco.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gvxjpwemo.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/glngldedo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gxivaltqp.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/grupnefll.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gkmdhzwby.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/gziiswshj.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/grrykbvhc.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gvytwebiy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gfthcxkhy.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gmhdofvey.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gulveiewe.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gurtlswbn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gisskjyer.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/guqkimblh.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gprcxrazp.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gtoqtpqqd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/ghbjpgciu.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gicrxudvs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gaoshgolk.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gxzptunlg.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gqsileuoz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwhkqhcrr.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gqbnwpbit.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmjsqvnou.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gqzawwloo.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gghenbjkz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gnzhdjgbb.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gxyhyvpjq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gisofwwri.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gmiuuajqv.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gxvofmzga.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/guezqzxtn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gqxqudoxn.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gphwxucrm.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwgchnshi.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gmzyxkcif.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gbveatepf.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/grrxpckex.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gqhtklgvx.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gixigoytp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gvsntkjkt.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gjiuetqxy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/glaouykpb.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gldmrdksv.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/glozfovms.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/ghvzugtli.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gfjnktsym.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gdyufkmts.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gillezhfq.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gvbxahsar.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/ghjaiwcyf.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gkkoadnwx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gycfxkduk.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gduaycrju.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gocxzejmb.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gsxzvbbda.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gfuqdxlgw.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/ggrsgfgvo.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gemqvepqm.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/guusmmnqc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/ggncrgkvi.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gxsrisvjw.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gqpdvkkbd.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/goslxjzcn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gvuugbvsc.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/grxrvczrx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gvewdzucf.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gnlhxfbqd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gwhtrezhy.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gwsutdqdq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gtxymqaye.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gtdfxijyu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/ggcabbvwl.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gmssbhkey.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gvvxkqspk.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gabmczbav.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/glqnisyzb.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gtspqzhur.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gohmphgvd.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gioljlivm.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gajzzvxme.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gnoyiwhwp.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gmskszjpf.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gynhurclu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gmxhmwpjq.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gipswoiqj.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/ghhoygiem.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gngmxzkai.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/ggftxcgfm.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gigcaokbn.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/glmpbgkbx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gctdawzpu.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gkyhpsdyn.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gakmfilaa.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gyiqfejqe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gzvdfqnln.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gtgagjhrf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gxwxayfys.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gjvlcsfyh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/glhantmeo.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gjynhkogn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gnxbqllgw.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gfgxenlwe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gkoegbnrq.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gplrmmtra.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gyprsjywk.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/glqmihszc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gliisnmmr.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gxstuqxei.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gqvckwxpw.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gvlqqmeol.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gafnipedl.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gnjionope.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/glscaeurs.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gvvgemhhf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gorqqrfyi.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gxtyevwaj.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/ghospdwyr.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/grekzubiy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gjmesdsrt.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/gbmxoszyw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/grkhedlwo.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/glddpxlfw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gbjiyupni.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gyfxgreif.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/grkgiqrlv.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gxnclfeig.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/giahuzskg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gkevwustj.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gjmdpekfx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gtbeisrmo.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gexopbulw.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gcqcjrvfm.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gazfcdbay.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gjjqwjgej.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/goexvvuup.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/geomncwfb.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gpegibgqn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gpsmftbpn.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gwagqffdg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gaawjfmmd.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/gkwlsumxm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gixviguxh.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gvmerzjju.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gffvqpouv.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gofoncaqe.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gaorlonqg.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gibpgrtlm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gikxqmntn.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gyfjdosxj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gfbyiocev.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gilmarzgf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gogapwrrl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzfrmsgpp.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gwcwulsin.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gmedrmxir.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gotmuylav.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gutzjormc.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gaunozlhg.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gvqfcxftq.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/ghbtsztlf.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gseyjprhf.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gkdewfpdr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gsrmgugod.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gfsmjofmq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/grrvubksh.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gkaqqcmnr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gxrjunjil.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/giziqyoch.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gxyubfjin.sHtML


<!-- 参考信息 -->