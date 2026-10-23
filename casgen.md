代发 wailian999

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3cjgjivcz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3bfenifnl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pafmrfvu.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3tiakxssd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3apkgimcr.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3cmbqvxzd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3ynajnive.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ctqqzrto.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jaonajcq.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3goxyhdwf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ketxidql.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3kcbblqcg.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ecglkcbe.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3uesswysk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wwpikkky.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3jwqlxwnh.html

esac
来源：http://www.52xcode.cn/Article/details/gt3jdjeofoe.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3uestficg.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fsrcmbex.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3dwqrcvvu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jwxmtlbz.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3zqjlglhc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3djotraqw.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lznhsaex.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tihscgwp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3bhcrlepe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3znpdngie.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3cnoaulrj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lngoxknn.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3axavlxmn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yopakiyn.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ogjaoiyi.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fscultfw.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3jaxqxhui.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3knuvnmdm.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ramkgkjv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3pelmeshe.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bpievfao.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3kzjsdmrw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gelzncxg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ohmpkaau.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vhdkwwrf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3hxftyhsx.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ekrsvvkh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3cmgqqcdd.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3axhxixuy.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ebisnpqh.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3qigunofv.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ydwqnrww.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3zdzbtwyz.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3irnobobt.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3twruuwqe.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3nfemhzgu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3roqrncak.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ipldubgp.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3wfurqdjc.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ubhdpkul.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3hgixvzbr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3efxduvqw.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3nexgpfcx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3fnryftlj.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3reesmqlt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3eqoevmhg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mrprvjdx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3umbppldm.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3lrygpcub.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3fmboszzl.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3dwphduiy.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3dkihmszb.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3hiohjnbq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3dvxblhro.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ucydzaqi.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3nulljahz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3gdabablu.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3okuxjwtn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3btvtzyde.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3dwkrmrya.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3rvcdgtom.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zeptzuwy.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3jrhsxxpz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3xqrlgvxn.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3kfgxvdyr.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3cnzlwflr.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3lcowvgtg.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3frkwhqzb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3qijcxesb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3wqxcbvux.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3hbvowmzi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iyvsutzd.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3tnbruhwg.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3syqrmgta.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3nyjtuojq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3vytkrmis.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3xouxmcfm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vedmwddq.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3jxppofez.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3wjnhmpuh.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3jtobmxnx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mhpyllow.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3iijaxdab.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3bfyfznwk.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3oarkaqlg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3drvnaujk.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3dbihevjn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ogrvhoky.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3cfxkqbou.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3rnmzqnfe.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3komqiaza.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3aizvjgeu.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3yedrkbkh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3pnjwyflr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hlapmgzx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3qogjczed.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ajmbrfpy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3rxrrqixl.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3zrgpdcut.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3zrjietyg.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3fblsimub.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3duqgbtix.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3qpflkjsh.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3rvxvvvgc.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3pjqfqopw.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3xwsyseax.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3zqrljvax.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3uzwwbabu.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3czxomnyd.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3tfzeinvc.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ntizgepw.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3clplqaon.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3mublcxsx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eocxouel.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3vngcwjwj.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3cmhaedwc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3deoobpww.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3gcljpunx.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ijlzotsj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3rpgmjqmo.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3dadhflsa.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3qivkugfy.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3puumfumi.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3lkuxbpzj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3nxgcxazb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3bmxwidnm.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wreowoqo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3cwqelxne.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3oczcmaqv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zsiekkam.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3enarhpai.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ykltkutm.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3yzcbkusx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3zweavthg.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3auezqiju.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3vayxadxz.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3jlomukws.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3cjkwfria.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lnopntab.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3afbmcagc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mvzdxvhe.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ndfgbdft.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3rojeazkl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ecjgjssi.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ankbaxch.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3pigtwplz.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ufunaufn.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3zbvbeyhf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3wlarmree.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3njsensbk.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ktsrywxe.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3nuqxcpea.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pulttjcf.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ulfboznw.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3yvwzgacr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3tnntsuif.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3stqcvdwn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3buucxroq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ixmvdfwm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3bnlppkkf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3lsuhofka.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3igrathzt.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3sxxrawan.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3eaiaaltd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3gjlnzeck.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3atpudaro.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3xgegnmes.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3adxriuur.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3wwxltxwt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3blvqbupn.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3nmwslfzj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3vxodfujp.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3plitjwdh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3qwmdpjwt.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3mwatoyxb.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3cocmxpdg.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xsmtovpp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3zhkzhqsh.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3yezmwvjo.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3oatpyhhp.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ocaflxfi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ytwpydkk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3pthbidjp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3cvcqiyha.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3nysrunhh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3euzztugi.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3exrxybbe.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3behksqcl.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3cbjsujlk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3cgmpqreb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3tfwcxqus.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3pbhmhlyx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3dkpzakvl.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ujmelovm.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3napnmols.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3hdweodzo.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3pbvdtexr.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rxlxzump.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3dkrjetvh.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3kvghjdjh.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3oetgtcfo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3bhtmedne.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3lrxzzfwl.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3sllsnvss.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3eoymqlif.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3rfovxljd.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zddryawz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3lefvkncf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pggczpud.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ghymhdpw.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3lamnlpwz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3obbnoxic.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3sdtvoqfe.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3iotylocs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3nmxtsfby.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3qdwbglyw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rrgrudbe.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ewbhpjnh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ypmjcnnv.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3iqpgyfxo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tzxvhocw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3hndionnl.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lcugyhuu.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3zefrhluj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3szbykqol.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3qbxrxkgl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3nbccrdou.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3yojcomrq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3mltpjtqu.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3aaxmvsdd.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3gxmdstry.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3vrjveqvr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3aoywxokk.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3gkxtuwcr.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3emeypftr.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3qhyzzfna.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3tdjtiwvc.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3lllclums.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3taugcipe.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xnntzshu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdfqodhc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3utzgeynk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3autadywy.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rboxlevu.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ejfrqpop.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3lsbdbahu.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3pwylavzz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mveicaus.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3sshrerrf.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3sbbpsflm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3xtjpcsdf.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3gvsuzsiv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3gcuanvro.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3uabfibys.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3gvsswqgk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vkhlwwmd.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3gbnhqcrb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3czlvqgwa.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3xyhwoivi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3cwxalqqw.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3vrbpbjjy.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yiyfapwf.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3apyraaos.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vcpsikus.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ocmqutvd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3emixfcro.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3mhpqkonh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ispdhgck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ctgxndkl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3zvzshpkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fksjxxay.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3edbnkwwu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3exjxzdyd.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ocxxrnma.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3xcxjtpuk.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3cgqbadro.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qiwvjqwg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3yxojkxkw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3rnldejon.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3fszauiid.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3zluouune.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wusirvpy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3proqvfjg.html


<!-- 参考信息 -->