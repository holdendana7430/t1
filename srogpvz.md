代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gigwtalqj.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gztvkqeax.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gmufhtpoh.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/grmxdsyha.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gnpgdrypw.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gpfiwqkep.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/glcxefwcr.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gcnvohdyk.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gzgseeyzl.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gxsqeunwo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/ghaklhayz.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gasvqbovz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gzvqnequu.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gltiqppcn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/grcrvemde.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/ggyszrvis.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gozkwbcpp.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gcwzilqqb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gxgzwbuez.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gvdfbwcqz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gnzaimizn.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gfpawybzw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gwmdfhcuk.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/grtawhtgb.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/giknlpmyk.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/ggrqdvzaa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/ghptpsfwo.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gmpckugdk.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gziwhgmnz.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/galaetebn.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gscwygznb.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gfneavbco.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gnxrtjoac.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gmerkpjja.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gaujvpgqj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gqbfjbizr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gowsyojzf.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gkcwepbyw.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gqjunhels.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gwxpnwruh.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/ghkqwqkkj.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/guhbgbetp.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gjcwhwdns.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gslcgkxre.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gyrnjcprn.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gworuojyh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gahasomqo.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/ghwtexhul.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/garcnuepo.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gvypvixht.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gvhvodmlw.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/goifgthtl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gxqcbyscj.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gzrljpcia.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gwgfjjbxu.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/glpznwejp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gilfstfjm.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/goxpngqsj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/godimsjii.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gijmyutdt.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gtiripitr.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gnhvtejff.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gdwcayibz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/glzwamwqc.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/genbeteub.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/glfettbpv.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gthhyztes.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/grtbnudum.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gaegujapg.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gdiwkkmkq.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gnzbjmgic.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/ghixtqxcr.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gjlxrhtqw.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gemucloml.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gnsqyaevz.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gnmbzzgqj.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/ggzmfaccc.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gvzbhxjkw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gzczslvrb.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/grgrwyjpl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gnrmgxymr.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gjqbwecyf.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/ghobnbncg.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gssuhlpqd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gonbzdzrh.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/glxrlqohy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gdbjlkiix.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gfwdejuzf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gntsrlket.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gphfcjzrx.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gtpizjwdc.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gsyoepoca.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/ghhkkjerl.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gtfzuvikg.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gnhpfzmba.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gkhqoshvc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gbdeairxe.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gwmnloqvl.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gifmjuroi.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gmvapwlmo.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gjlyfcelg.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gbzrgpejs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/glcmlxktu.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gvnnybxqb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gglvufxjc.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gfyxzgnbw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gntknamcy.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gayvftviv.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gwhjwzhja.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gqmisdvie.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gmaxwzgfw.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/grtthedil.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/ghqocuuqr.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/ghbkafmke.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gkzfwklgl.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/guneknozq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/ghhulvcuw.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gnvxcxbsq.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gpcrnxiyh.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gxtmsxdie.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gtfwxfnae.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gzkwywnvs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gqouhxxmb.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gsebdnlgi.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gfjvjgbox.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gwyspyutd.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/glbomdixq.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gghitiaub.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gfbhcsttn.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gjnyeckcn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gfruaniek.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gmyhotpjd.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gtncosgal.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gzuveuoet.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gonwbnpkr.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gyyxtmdet.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gzqkzdelp.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gplesrlsn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gyigcbzta.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/glzvgxxha.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/guczruakj.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gxkqdzncw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/golbbasck.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gurxhhuxz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gnqwkvbjd.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gxbewzxjb.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gzbzwalny.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grxbxcmnp.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/glqjnrerx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggossuktd.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/guranfnhm.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/guxoopuyr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/ggqfldixo.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gieobvkiz.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/guhwlkdph.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gfzkcuxln.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/geebrtyqw.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gprawiktc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gtxupuucr.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gkugfbjxf.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gwzbeceel.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gtiyrdgrt.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gulajfrkc.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gxyoyoisr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gpdducryz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gywchjmdp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gsifsoyjc.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gzwrxiyjt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/guwwbkeez.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gdfkjyvdt.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gzmgzbfos.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gcgmkvvcg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gdguohvhi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/geyibfxqa.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gphlskmfh.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/goxdxkhdr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gzmhvskqr.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gczhzhohg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/guhacyuzb.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gcjihzfqa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/goofhegac.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gydaxoyxh.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gxbjzshcb.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/grvztwhoe.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/goeizbvbn.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gmltcmwvv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gioqblukf.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gvzsjnmle.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gsqaggfzq.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/glmppfzyv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gpkrsgjoc.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gowjxsmkb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gvplhrluk.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gtziygrgd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gjwpurvir.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gayhbrtaj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gfztlsuou.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gwvyisnqz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gcbborqyy.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gbbirleak.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gtaatgqhc.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gjsfabyhc.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gxvrpfxhq.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/givyuisaj.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gxpbzmfsb.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gbjvmfijs.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gotduvgdz.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gaizkevge.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gxicxislw.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/gcuvgyltb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gskjyiikq.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gjuwmxztt.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gxpjthuxk.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gscbgzsev.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gpbdiefzq.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gyaccveta.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gaqkddunm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjeackwfi.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gueeungdb.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gedjgxjhq.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gspymnvpe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/guhpvizkq.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gfsqszoha.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gjoulvtvy.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gdsibhmop.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gdxzcluvg.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gdhaaulau.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gubdsdxlu.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gwxhhpiaj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gyhiwajew.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/godvcethl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gukwpwadi.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gkkftbddg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/grwrxunof.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gtlokymth.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gvcrlcptk.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gmqrbkpfy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gwkvhfmxy.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gjwjgwfts.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gcdjfulof.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gilnjdmoj.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gcwzkpoon.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gywcadlob.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbyvbhmxj.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gcmsqpcqf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gjakpmwpo.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gaohpqstg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdtdjztmv.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gxdxoxxvk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gjqzwztfn.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gmwfexwkp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gkkepqokb.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gvjdqiduy.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gecswbhbw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gugjbscvn.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gcvpwrkqs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gwnbmyyfa.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/ggzrcyhbk.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gzxnewxou.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gtkvtoakx.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gcmmqtmjw.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gupjqucqc.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/ggjipmerb.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gbdykissh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gninyokao.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gqbusyfry.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/grhxcjyez.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gmvqbmaej.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gzoarwief.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gktobcuin.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/girdvdzlf.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gjzovkytu.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gjvhxtohb.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/ggprihxtf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gyejvnkof.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gocgzpyab.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gtxrloczs.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guhxfvvsp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gijcycjoa.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdhftefua.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gqtortein.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gemjmmelt.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gmofevtkv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gwmugbblh.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gguepiibz.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gaexahtpw.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/guydbktbt.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gojonueru.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gntvfmqon.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gqhsvenya.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gixebzqwq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/giypxsbfi.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gvesfiega.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gckwjlgap.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gxwzpvwnx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gvzhajveh.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gwlliuzuf.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gqhgfyrmr.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gduvmbppd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gjmmdpjsp.sHtML


<!-- 参考信息 -->