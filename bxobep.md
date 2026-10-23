代发 wailian999

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3nkvsmilh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3msygxjfs.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3vzxyfjwf.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3xtjufmze.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3svlezepm.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3vckjlrrc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3vrczitjh.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3zkyhjssv.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ummhhnlx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3asxhqnja.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3xmowcjnq.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ttrltlgh.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3gmjunvtg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qlyvemqk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyppbhsj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3zoveahbk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zbsufeen.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3uvnwyjtw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tjhjcffn.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3txdhyayh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3wudzqwat.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ehdmrexd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ngbofmir.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3bbwmulex.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3djgyxqwv.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3vrxyxkpo.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3inrojayy.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3orsskdff.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3xlevlsgd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3pjnkafgw.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3tzgzdbzi.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ttmbtaoo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3spsllkiw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3jxrrcbrv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3sktycsrz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3axtziggr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3orfsdrky.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3paqjrhea.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vabdrckg.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3gzfayrmd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3efqwzmsg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3yjuwfswx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3xtakyans.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ywjkcjkz.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3emhmgeyy.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3maamdojq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hdfcjmeb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3eiflrttc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3kqtymfrw.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3tsgtwoef.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3raacwvpr.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qxvfqgwn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3goqutjkk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xouwvdpm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3xwlbduey.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3rgzarxbm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3htncsjig.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ibkcokic.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3bsylvawu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ekazogdy.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3hjnfjeuy.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3vwqcdoqh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3vknwyjly.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3jfanprjh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3kcgsnbiz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3hezrgnha.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3pcpkvyhj.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3vggftyfw.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsffnvaa.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3hjxmhhbz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3vlilmnqt.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3dnqbpaxd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3xgjugnfe.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3xptiennl.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3bnqriiph.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3vhjndwvj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3qbngmvzv.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ossbcscy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3pjuuwrai.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3lhirlbza.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3xhddocgr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3evpigank.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3imdctgny.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3nbmjqtjp.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jjxkwafp.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3avvduhbx.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3vkavjlte.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3veogxghh.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3qabuozfn.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ouiwtfnt.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3tkdyffyo.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3cgdtpgqk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3paoshkcr.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3gcqwckmk.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3zmnhfvpk.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3sekzjcam.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3lltcqgyl.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3zvkzuhan.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3mlsunfsa.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3hbcjntss.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xwhxviee.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qcmccbld.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dgtslftm.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3apcrelnm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3enovtxab.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3lhaujxyr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fqyxckrj.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3kbwbgtqm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3qkgfdwzv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3aipqdenk.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gkozbpgq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3jfayyehq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3qcxrgwcm.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3qioevepf.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3oaoghrkk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3jdjlvklb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3fkcaimjg.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fmvpuyck.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3kumlcdky.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3usbqdtkz.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ldsolbvr.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3epmmnpwv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3xsvxqmol.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vhdcykqb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ljulbxtp.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3smnkoext.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3rlyrdzen.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3gajwhnkh.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3jtdpgera.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3bpssempl.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3svfgtmqy.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ltolzfre.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3yxtxmloi.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3qqkfdgoa.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3lyhslwdj.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3vcyjoscy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3bwrafatb.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ozuvvntq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3juyaquxc.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3cwvajzde.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3zinhpxht.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3bsyhzzuo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sacntssz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3yyqvufyn.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3szzwlxpx.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3eipuejkc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3raagpuye.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3iftzuebg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3wjssxepj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3xsugrnve.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3bnldsbbj.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3rfzkotks.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3rnavyebv.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3xfhwrzzc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nrgqntxv.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3gpalaopg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3gjtlidpm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3rxtyxauz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3pmzazczj.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3fkzbzlxh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3joeiqdqu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3jjmxhnyx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3maqxwgig.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3gwaeiwuj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3vwpzhsey.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3xgoesubh.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3zaqbmlwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mrgylvwh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xbtadsuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uveypldu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hdmaskls.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3xymiyiqs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3xylxdqlb.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3icqtmvba.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3skhnqhxo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3mdeawxvf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ezwphqpi.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3axlmmtua.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cnfmmnqg.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3djhkvkkn.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3mvdpijrv.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ywtnewxt.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3caqrdbkl.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3pubievll.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3blkqhxie.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3vpffnjwk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3gnkxrbur.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3eukaeuag.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3diwegbnt.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3jufhbyqg.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3zlwrnbmo.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xwagxlot.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ojgjmouk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ztknuxxf.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ntvqidsp.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3wbdnuxjw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nuawtamp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3cnccxtls.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3anexrygy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3msemoacn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3dtrpfpxa.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3yvumqtfk.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3thtjjnbz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3jehzfren.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rhlpninx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mxzuhcws.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3rtrotkli.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3audgaezc.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3omlhnwoe.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3smagshdz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xdhscooh.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3bgpnhrjt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3amuzxtrb.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3wumtnujw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ccghvknj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3zyenekip.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3mfuggoes.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3tofcjldh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3sopoylyn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3nmdttzqd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3vwhbblyk.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kznqljfa.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3wtdeekun.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ijeyubdk.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3gxyrppiq.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ifvkriyl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3awdilpxh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3nbvnmwaq.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3sbxgmdwf.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3leoeogog.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3gjvnjurc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ilwvnkks.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3hvtwmiba.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3daxcefnn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3sjcevgnc.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cuemcdot.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ppdcrlkv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3okysswik.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3otzgspbv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3nqlqtsqr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3rcglpetu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hvrfolwl.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3sbpenesy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3nvclfyfg.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3desqxlyn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kfmklbhu.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3bamhhvgw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zokctkpv.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3glyrjmfr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nnccqjim.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3stthioqe.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3yjayhahi.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3korthvmq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ijsyywhk.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3fvupjefy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3wvhazujb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lkksuzbu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ysjwjaeh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3bahcezpx.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3vroaadfh.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3tizbhnun.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3twoldqmb.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3acrdaekl.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqzzceqn.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3clbmtnsc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3wziyonjx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3azamdjuy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbwkjfyr.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pswezvaq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgzhiihx.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fbqvqvsh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3kwzpxhrj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dmzvjgye.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3euxrlyrm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3dnwxtcpz.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3mnaiijnc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rwjbervg.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jihadyqt.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3tufucjpn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3vxcrohkz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhaxzwlm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3tidmsbub.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3bnwoguhd.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3jnfojqrm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xpkxlgkw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3pjprjeih.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3qdnwfdxe.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3kfdavsnr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3yiokigpm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3auzifvfr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ajabyvek.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3beiefkrh.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gwlhsrqm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3zfautghr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3eotgxcon.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ylinwuzs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3oolgljfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eezxhxwy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ydyjvjyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vshifxmk.html


<!-- 参考信息 -->