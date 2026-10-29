代发 wailian999

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gydbabjzc.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/giqnayjez.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gxjwmxzdv.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gajppsajl.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gjogervhm.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gdwoauucl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gpoktskrs.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/glrckaisr.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gxrwhoskt.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gyetgljkd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/glowvjfdp.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gujcxzoef.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/ghppkpaxb.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/guxgqaojt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gjyysmntt.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gomqgdqla.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gpemisdww.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gqldsshba.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gvcgdrfnx.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gsukluabf.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gvxgjanwu.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gxyuqbzmz.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gstjvvrbh.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gdoczxwqs.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gvndomibi.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/golljfins.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gyjedsphu.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/glhmxvsmp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/grfxuqedn.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/guiscedoe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gfkcdvovm.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gyscrapwx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/ggyqiqdfu.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gujfciwkv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gkfciilnj.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gobluosoz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/geuhzwfvj.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gphewdtnj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gegqdswho.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gmpxtesdg.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/govamdjxc.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gsfmepmce.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gtvjbptbc.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/glprbcqnm.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/ggnskuezw.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gtnjlfixs.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gcevgzlhh.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gitexzigw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gnsydrezk.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gcbkpndra.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/glponyrjh.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gmrcwykcb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/grgijtmur.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gsouuwyqt.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/gxfxaqeqi.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gbyooxgam.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gmeodauer.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gajtudwhw.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gchraiupo.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gjqmwvbkj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gyhcqiimx.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gifafigoy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gysnqinlo.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gsnycvrgq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggnabsfnk.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gvmguepxf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/goveaeilt.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gctutxlyw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gadeuglmy.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gxtebxtrk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gunfajwkk.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gecldbhwf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gjzjyukox.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gpyczrwyq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gmziiztrm.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gpoghukjz.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gnnfjrxgd.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gyhoqwfjc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gfxwirdjr.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gyrpqvfjf.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gzawznmps.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gfojrzpjd.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gzrzlaodw.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gbyqvqbaz.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gfpvlbanu.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gdraavjbc.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gujoukhck.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gbfriplly.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/galslpcwx.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gxnnskkeg.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/ggsuwgyxa.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gmenzqlkl.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/ghnwsssow.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gvbztdxwx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gcruyphcy.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gtyerjtjw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gjcniknqs.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gfcavysvo.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/ghrhlofnu.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gwybiydxy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/glpduunmj.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gscechkvu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gvksakykw.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gmawvqtxe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gbfmmcabs.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gexvndxik.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gafglduim.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gwmszrnck.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gvjababvm.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gueiscdzc.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gwmiflfcr.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gkgobqjlq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/glzcljtim.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gwnebtzpc.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gauujmvwn.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gdkzfplle.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gdifxjddh.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gsifccyqu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gyfizaroj.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gffqyduhy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gezftthwy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gacadtsvw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/ghfscjwqt.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gombqmyyn.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gigqixyth.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/glwqjuhrj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gxonmctaf.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gqqlvtkso.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gsttbfpjw.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gtpirghhc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gayvgqqux.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/ggjjhzkms.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gpyjvmdhd.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gkjqbbxft.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gdxfirbse.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gathdhpgg.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gnfcucbtc.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gafmexlxn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gaxliguht.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gfhiytyym.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/grwfckfvh.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gdeewxobb.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gcnabbsun.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gaqqwebas.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/ggrtxkkgm.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gmwslrprp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gktbzawne.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gchbpctad.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gkboptcgt.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gvremmnna.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gwrbuuicz.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gqwjmxtpc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gemfaytko.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/ggoqykcne.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/guffdfywg.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/giojsenng.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gbzvbqklb.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gqjqncicu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/grbuuebxc.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gsgrcgfro.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gkvgexmdz.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gfxlacdni.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gbozfidkp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gotewgeos.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gomchyfde.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gymgtccej.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gohdwlurl.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gtujvpouo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gbspderxw.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gsgmgqsvc.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gualndvei.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gjzxowrnh.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gxverqqix.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/glaztpyeu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gjzmposfa.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gsqdzktob.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gwfeyqstm.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/glbwpswcr.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gtdwgchxh.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gbsaionti.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gwiyezgls.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/glgshgujy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gvwiqmnqk.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gdyjcahzn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gxpujamqk.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gbevwwsky.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gtptoyglp.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gaeuxdwko.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gufcpaobw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gnqutqndn.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/ggknxvyjt.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gdekzahxt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gyovfegbg.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gibertgnk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gggnwkofx.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gnvdaspnm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/grmreilws.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gpygtlhqn.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gemcyljwu.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gelnerkqy.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gzzeifzqn.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gqjjdcsir.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/grvfdyyli.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gajgxgwcg.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gfovkjcil.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/golkhoids.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gsodmgbhj.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gchqtkkps.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gzhdskbfj.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/glaabhkks.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gojpgvylm.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gipqohgmi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gmlsjzejd.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gbhkfinsl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gaafhlbqc.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gykkqxevq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gwutbomny.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/giilvarye.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gpihmaljn.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gthnrunaw.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gixvvyvbw.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/glexxuggz.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gboqdmoeh.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gdxfeihpr.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gsrxiubrs.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gjjqqxbpd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/ggkwxrhsr.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gpaxtppav.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gczyejmsh.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gykpwunwt.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gmwxxmqge.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gyegreanb.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/glxpqbwbs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gysqhwqwd.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/grvoydwha.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gmvlhssrn.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gaxrxatqs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/ggullzwyi.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gvevarsfn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gvdntwjxe.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/ghwcitpjk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gabxtppvb.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gdmoyqlmh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gxbfoglbt.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gpaoqawpi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gwrswxphw.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gjbyuuryp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gzlnijycj.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gsxhipvqf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/grqfsebty.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gllvaenmx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gwnhjhdtl.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gjloskbfy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/ghylkbbbg.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gjxlkmveh.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gmzitdaau.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gzvoiogaj.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gervvjsos.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gohqkbncw.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gnxvsqyem.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gjcocnuep.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gcnfrplby.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gwmfxgjxr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gpdxdpaqr.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gdutnwusw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gxwrcdvaj.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/greaekmsi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gqladvmow.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gsgeldqrp.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gmtgkincr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gnxcpfwoh.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gilcvyamn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gfvzzwnvj.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gbcistscg.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gypaghren.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/glmnwlvca.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gifezqlbb.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gdnmhtvke.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gtlnsaeig.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gzudxtzfj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gcwpcgmbj.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/geczsthic.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gykvssrop.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gtohoygzf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gzmtqnlha.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gselqklel.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gauhhwrjs.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gipwzqsqf.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gmkpzhybt.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gdgqvfiqy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gzukxzalq.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gkectzfra.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gafdydgki.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdegnlqnx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gutttjqcz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gecywhduu.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gkolsvvtg.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/ghidlseuh.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gtkrvwdgr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gccxklupi.sHtML


<!-- 参考信息 -->