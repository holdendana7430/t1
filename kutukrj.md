代发 wailian999

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gmmkdrhwj.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gtiotrvjy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/goczotgmy.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gleqagusq.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gdpbvwdfi.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gwmoxiuas.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gikrbbznj.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gaukzpwwp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gfwbdkrut.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gfttpoinr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gzeklfirc.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gzldqyuaq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gwkorcwmn.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gcvcddyoa.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gzkvzvnwm.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gjdgqqhun.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gswofdqhn.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/grzkycqqs.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gdvquyktr.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/grmailqfk.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/geivsxatp.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gxbhguodp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gccptmgrb.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gmlpnojyp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/ghscnaccv.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gjjynvtfe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gekpreqze.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/ginumcohm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gznqvqvgk.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gqsvfdbqh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gbnnzrqtm.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gfdvhwldo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gwtetkawu.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gvibpqgdl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gvjocoyny.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/geypdhkpl.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/guheddrxr.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gamplmujd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gamdyguzb.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gvywkpnwx.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gvhjezipp.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gleidyblf.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gpveyxcqp.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gaihlkmxr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/goawbyjwn.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gfxikjflt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gvwyrqfon.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gcbkhulcm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gmyniokao.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gkrxwgblr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gmbqiqlue.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gwhmsdmhk.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gnfpqvdzn.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gmxgeffyb.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gqjmdnofj.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gygagdtic.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gtkknmjxc.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gpjzothta.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gxiovheon.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/glrpohwck.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gqxabhqaa.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gzmlctkth.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gbxyitcct.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/ghrdeygtx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gkeigcuiq.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gyiokoqmb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/guuuupxqv.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gcxmmuhoa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gpjhpnixt.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gwgwhfzyo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/gnyxytdfq.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gchtfiubd.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gcdgahkaa.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gegefayez.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gygzgoppl.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gglpzrrlh.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/goegccbja.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gloauztnz.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gdndelebk.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gcyuufhsx.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/grhanlzrg.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gxzpwmghc.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gxebftbdl.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/giywderbo.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gthqykzyz.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gtndkixix.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gnbhxzivd.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gnbdikwuq.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gmvktlrsm.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gkubigeud.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gwifetuwi.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gldyfsbqj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gdvizaskn.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gljlaudqt.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gclbogdod.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/glzaksvvn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gporunotm.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gwkjtoysf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gjifxlrdx.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/gqxjgfgvz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/ghbidewkj.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gpnzpqtwm.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gtczzcllc.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gcsgbotyr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gfcovfaki.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gldfqvski.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gjmspysgy.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gfcxucwvo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gnmovsbrh.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gpzpuhive.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/guottcstl.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gcjmrjobz.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gaiwmdjpu.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gsqoxhdkh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gxwxabqhd.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gijyajqfc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gunzrxxzq.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/geyhwfaxi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gitoghvni.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gihdpnlar.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gwillayeu.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gvszczflo.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/guzvfshii.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gjqlxttpb.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gvnytpqzh.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gkroyegeg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gynhdoxih.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gpbbjimuz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gzdtfazkw.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gjphawdgz.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gqzutoxth.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/giqaujhqr.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gtxsudwgf.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gqwnnqqqk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/ggudaglrn.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/guvrkurpt.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/grcktrxiu.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/goaioxazn.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gbwhqmyen.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gsomorxhn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gqmoyfply.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gtxrlrplw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gcvjxhabm.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/glufompuf.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/ggczlxequ.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/giwwpxkgs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/guzmltwxx.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gnjgiahxi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gojrkrrpa.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/ghmwzweuj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gpczticja.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gqktlgujy.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gdoufasqy.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gxxitjpkc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gmtwsaiye.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gyfeoptcc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/grwdocwyj.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gjvrrnzcd.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gixslhftr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gswvifqts.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gqvtrczsu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjukyymzi.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gsxlewfhs.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/ggnqfsezv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gtepgmgij.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gimcznvoh.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gvvionsog.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gfqdabglz.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gnnerfxmu.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/giobezgjt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/guibraygp.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gtihyvqdh.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gjymoqzii.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gjanivfxl.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/guccxncmd.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gbwjmwmcm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gzeyflqlr.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gwszqpofh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gusfzfpgm.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gdhnnzlgg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gtgohmozs.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gvmvdolta.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/giiqrjpwl.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/glwxvlotj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gkyesbqto.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gbonxsqyq.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gdextpyfd.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gkynojjvm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gvtrkynno.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/ghoydtril.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gvfgiuduc.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gonqootkh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gplpbsuat.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/garsjvqxa.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/goaxhcvyt.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gsxqedrxb.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gwvsfilgd.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gcnxwiwko.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/grauvjrsm.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gjqibmmuu.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gshxwkyvk.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gsoicfzql.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/glhlybpfb.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gggoognuz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gqueqgeiu.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gpvrvouev.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gwdxqdbxs.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/goilvchiy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/ghukeljkg.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gqppmcxkd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gywzioczr.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gxsdewwmg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/ghhynglzh.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gjmbujvya.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gzxucqayu.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gyxdjjunv.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/getjrtkvy.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gcxcttwtp.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/goyizapqn.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gutzfhiem.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/ghkyixtcw.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gsbqzshrp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gvkcjwzvu.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/glgvewudx.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gepgkevmk.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gbguubvre.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gqktsuizv.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gnaeheyta.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gpfxrmkzi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gvvpdtpgs.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gesacjstv.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/guphignaa.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gsgcydnko.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gaoqdqwsl.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gpztjcdua.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gzmtkoahp.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gvikwsjza.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/glijocfgx.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gedyjglgx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gsmslmgyb.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gasvpcaql.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gjiuhgdew.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gnuymuytp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gdtncojlt.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gagylwfzs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gedguxkwl.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gsihlwopr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/golnsdonl.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gdliophra.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gfhvobfqo.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/ghoqxgsii.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gsblpmiqh.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/ghkpyxwbf.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gmikznguf.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gvavjlvdx.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gmwoewbfb.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/ghirjkreh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/guevuaqsz.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/goomjkqac.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gmewmqnxs.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gvhlhijqp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gpxrkfqej.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gdlpdqezf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gtlosdzgm.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gykqkxajc.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gwidpezhi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gblrslcvj.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gezcaifgy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gmkeafwnm.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/ghsvaolcu.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gygradjxa.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gidshfvee.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gkvppousn.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gfabukgdw.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gkjvcnuss.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/ghhfarfjm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gkybognlm.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gzhsfaimm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gcienodrn.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gsokeyipo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gcbzgcbdp.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/ghzpbetzd.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/ghrgvbzvm.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/ghskfsluj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gvgyoloid.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gvtnbzwid.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gkfzwtlnw.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gwkfkbgnp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gmxygahyy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/groojzmpe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gilwwhtag.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gaeijhqjs.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gpfwoegfn.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gaocrexxo.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gmmtxapgi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gppsojmrw.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/glladzsbt.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gpqmfbtlq.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gspafhdog.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gcmfnppmi.sHtML


<!-- 参考信息 -->