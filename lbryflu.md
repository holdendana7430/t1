代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gcefrzuun.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gojhhmvzw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gcznwyoaf.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gyzjuqvyk.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpirdtao.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gpeuzcdwe.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/grmophivb.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gpfajzijm.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxtakbwv.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/geytvozve.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gnfzmqwet.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gyehjidnh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgeeaxyf.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwpbsafj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabefgtib.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzlypltce.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gufovtjbq.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gniqbbdpb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdkpzdpa.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjlptwpx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpslzlyiv.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gyevnpvci.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnypgfgf.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gswsdmmhw.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gxxmjwhaa.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyawmqae.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gavuhlxyo.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/grcskqfne.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gshrrsomt.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gdckrymup.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gsczasvah.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjjvjcmw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpdvnovs.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gvearwsyc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtcgoykki.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gkhiawsci.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gcrlvkzoi.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gtefuuuep.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gebibnyvm.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gbwkvmyys.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gdgxjgjqs.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/giqiwmsne.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvjmnaas.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gclntvgtm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxaidayh.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/ggmfmatxy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gwpgrkezn.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqgrhwnx.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/grkqxfkfd.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giajkjegc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwoumdegg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguncpjbt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gxrnwbngp.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gkmvrhfak.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzpokzha.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/giyvlqjoz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/grhnioprx.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gukifrmnp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/glzsouvpb.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosbhmlax.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/guyrmcfex.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsvmsmqf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmevjejy.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gotswffdx.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gllscsnpo.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfyfntxc.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gknhljdsf.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gchetevst.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfayiuif.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gswvthytb.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjscpdohg.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggssjjvng.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/glqusudwq.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/geshntkrq.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gmlzccvpl.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/geyukzioj.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gcxleadwa.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gjbbfabnp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqeqnlbq.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gjtcusknn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/glytwrfkj.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpocjaxu.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqiitdrqp.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsenbxbk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gqsdmzqun.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gvnkpruly.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gykilowzg.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gfucnrnyu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/goptoyhuu.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvkikwlk.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/guzmdiomc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnqvnveh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gelsjyhcn.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfiztjsah.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gakkcmyge.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/goewdnpwx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gpozptyxz.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/glpesfuxw.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gxxgdaadp.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmdubafn.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujkwycpp.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggucjkvtv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvqspfbs.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gpsakjxos.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzpxmium.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gzgolwetv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gurgrgupp.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gcthoovhp.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gufjkksup.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjrzuspr.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvkmkiuy.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqcdgfbx.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gcghnkjgp.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gwendbbkr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbvkjgpw.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmwenbfq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gbwuaoaes.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjbipwju.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/ghzqaytqj.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/grbtvyvmz.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpsexiwo.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gkaobnjse.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gklrieuph.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/ggayvkqss.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gbzvazbgf.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gyaaxjtiu.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhtivcgb.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gtoqivofu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvywcgjug.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndwmjzbo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtskfdwvo.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gargjnsxd.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntneohnz.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gxhqnopwf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gvalgqngg.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gupybaadt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gueimybsz.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtafrkzid.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyedaqqp.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedzuuzha.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gahnfeomi.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gjilkcrtt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/glkbfzeip.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqmiugzv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrbsmgsx.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/ggekaqnuk.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjtjwsar.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjfajkmp.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gpbrmhfwm.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfbmhuugg.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/glirmotbz.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gcqezujpo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/galxxikww.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gdnypqazv.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gqbckxwbh.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gubuqnbxs.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gadkfhfxj.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvzowhwb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqpbpkxi.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gfwhofybi.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gqimurbku.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gespgjtan.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gaeyappds.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gwqxqxjhq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gldjrdcjt.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcorlplk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/ggtmdfxhr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdxamdcn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gobgjwahp.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gkgxtolrr.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/geyvukpdh.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnfafpiw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gitljhqus.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtppjymux.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geomvpbro.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqngampd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/guzgjvdci.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gtifbxnrc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/ganoikdzc.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbugskww.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gubzjmitm.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgvilyze.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwvihrmq.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gvrmsgpxo.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzigjoji.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoasesub.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gwsospsly.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzevwrzr.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gvwrwwoeq.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjebvboe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gfumcijge.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzfmzvqz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsnoiccc.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gpnjbodjo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/giuobtyty.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/geyakjzee.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaedrtfpf.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwypbbdf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/goyzelttd.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gwikojzyy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gfhvhaacu.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gmiggiufd.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkdxkwxr.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gfzzixjlg.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goseppnkv.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gqqdfozhq.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/ghokswpkf.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gzcqutdho.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfawrmiya.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gujizptwk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/goapuvwpn.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/grluszhvu.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gofatqzgp.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gcprorhau.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxwkrwue.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gnelsixzv.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gqzgvibhs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gurgmedjb.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsudzkqp.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbnmisvn.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gcgxofzdv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gigvnumvy.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrfnpvch.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrtsglki.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvehyjpd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyycpifp.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gvhlcjuxe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gqpcfwjau.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnsesmwu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmxwbemy.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiaerotb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwcxqcpm.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/glyvbulos.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gmhrbcxwn.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gcedlzmzy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmnfrtao.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gvzszgkdj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkojvltz.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxzpmnmh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqizpuzbl.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyzqtvvl.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyoipczs.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gdlqouwrm.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdyvjyix.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gjvlzaszo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyuegyro.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gechkuuwh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmwranytn.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gyxeztdjm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvgwihrg.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkknbtyon.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gezoaxvze.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/grijryxxx.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdulgexgr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqolclxo.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/grczbqsux.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gxswtnbss.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbabsozko.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlzbvgwf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlcwvxio.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjpvtvkzx.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gzqfmbojg.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhrnwvpj.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gbjczxiaw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gtvolthzz.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnsmbqrg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvvrlegz.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwdaraea.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyhziivaf.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrhurxyg.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gihpxafoa.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyxugusn.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gtccsgagf.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcddakgsc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gagtbovbm.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gewowtjup.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gzmijmbji.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwiycwfwl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/ghfaepxwh.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gamlskddq.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gmwumteno.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdtswtja.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gksupxaql.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqrugvni.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gjaacyoft.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gkedufkmk.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/glmftlvmh.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrtsscfs.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gcnquskhs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjeeejkq.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gcmdwqwhb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxkiuukb.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhacqzcd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gxsaatzwl.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gyarzlxcm.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/goiblqoho.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzfacofq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gennklexv.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqtubdfg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gabkirtqt.sHtML


<!-- 参考信息 -->