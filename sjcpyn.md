代发 wailian999

R. Bash 专题
来源：http://hz.ehwqpu.com/gtjzdxgyrg.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtmfdpqjna.html

[R01] shebang 与严格模式
来源：http://hz.yonumen.top/gtvntdvfaz.html

#!/usr/bin/env bash
来源：http://hz.jinqigfzy.top/gtprjahtix.html

set -euo pipefail
来源：http://hz.pengpengdd.cyou/gtoejfhhqp.html

[R02] 变量赋值与使用
来源：http://hz.yj202588.top/gtdatytlwb.html

name="Tom"; echo "$name"
来源：http://hz.feifeiyinyue.top/gtdmerlxzn.html

[R03] 只读变量
来源：http://hz.daria6918.cn/gtcjzmpwdl.html

readonly PI=3.14
来源：http://hz.52xcode.cn/gtyvurgmua.html

[R04] 位置参数
来源：http://hz.tanke756.top/gtnlcjelwk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.gaohongyu789.top/gtgcfbwtto.html

[R05] 参数默认值
来源：http://hz.jyoumei.cn/gtvkpzmwuz.html

name="${1:-default}"
来源：http://hz.yvedp.cn/gtcqxihkqm.html

[R06] 判断命令是否存在
来源：http://hz.yj202588.top/gtekmcbdrw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ydzc1.top/gtlqkaqolh.html

[R07] if 判断文件
来源：http://hz.nanxinkj.top/gtyxxnqshm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.chenlongwang.top/gtfmevjxhx.html

[R08] 数值比较
来源：http://hz.aizwys.cn/gtvhrgvlmg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ehwqpu.com/gttdepnody.html

[R09] 字符串比较
来源：http://hz.cdnleiting.top/gtjlcmwyqa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.mhx1999.top/gtbuhatjxp.html

[R10] 正则匹配
来源：http://hz.yonumen.top/gtrxgiujae.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.gaohongyu789.top/gtzphjfjxg.html

[R11] case 多分支
来源：http://hz.snrcjt.cn/gtlgshgizq.html

case "$1" in
来源：http://hz.zycfv.cn/gtnldrihgo.html

start) echo "启动" ;;
来源：http://hz.smart0.xyz/gtzhjyvgfr.html

stop)  echo "停止" ;;
来源：http://hz.zhaomingkeji.xyz/gtnfwpihrc.html

*)     echo "未知命令" ;;
来源：http://hz.shanyushiyangtech.top/gtqhrzplmm.html

esac
来源：http://hz.vqdsnc.cn/gtbyldvveh.html

[R12] for 遍历文件
来源：http://hz.pycfn.com/gtltapbujc.html

for f in *.txt; do echo "$f"; done
来源：http://hz.tianlin.xyz/gtqmfltdkk.html

[R13] for 计数循环
来源：http://hz.yanxiufei.cn/gtsojmmpew.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ivvv.top/gtkrqjdcvc.html

[R14] C 风格 for
来源：http://hz.sysykeji.top/gtjhmrtqad.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.tianlin.xyz/gtfjcuonxn.html

[R15] while 逐行读文件
来源：http://hz.yj20258.top/gtofeebkdb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.gzhubu.top/gthdndqild.html

[R16] until 等待条件
来源：http://hz.ywan-chungtsiang.top/gtgqjppwbd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yangfankeji.com/gthpcukyyp.html

[R17] 数组定义与取值
来源：http://hz.dashuyun.cn/gtaewudcst.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jqgufenzy.top/gtlonnaauf.html

[R18] 遍历数组
来源：http://hz.wangshuangyany.cn/gtsymnjiwa.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.nanxuanxn.top/gtrxbgxesh.html

[R19] 数组长度
来源：http://hz.ydjk.org.cn/gtwzaxpepv.html

echo "${#arr[@]}"
来源：http://hz.aizwys.cn/gtczlkutao.html

[R20] 关联数组（字典）
来源：http://hz.tian-w.cn/gtybmxxjto.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xinyue.icu/gtzxsgvqit.html

[R21] 字符串长度
来源：http://hz.mhx1999.top/gtusgemqgr.html

echo "${#s}"
来源：http://hz.hfpthk.cn/gtexdmrbbz.html

[R22] 截取子串
来源：http://hz.jqgfzy.top/gtwwxcjxuk.html

echo "${s:0:5}"
来源：http://hz.yueranfly.top/gtquxzmmhn.html

[R23] 字符串替换
来源：http://hz.hongshengwenyu.top/gtuzljrwwz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cheryme.top/gtjtxjjgpm.html

[R24] 大小写转换
来源：http://hz.xinyue.icu/gtiivijkxe.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.chenjidiqi.icu/gtkmjfncqr.html

[R25] 去后缀 / 去前缀
来源：http://hz.aizwys.cn/gtzaxezudo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xinyue.icu/gtbjrqvvum.html

[R26] 命令替换
来源：http://hz.fzhhl.top/gtihhixldc.html

now=$(date +%F); echo "$now"
来源：http://hz.jinghuilouyu.cn/gtvcohejvw.html

[R27] 算术展开
来源：http://hz.svipenyu.cn/gtapujnnzm.html

echo $((1 + 2 * 3))
来源：http://hz.sysykeji.top/gtnjksxczb.html

[R28] 浮点运算
来源：http://hz.ywan-chungtsiang.top/gtwrkldsen.html

echo "scale=2; 10/3" | bc
来源：http://hz.ivvv.top/gtmeneopha.html

[R29] 定义函数
来源：http://hz.jyoumei.cn/gtokjxzxdn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xziqi.cn/gtnlcabcsd.html

[R30] 函数返回状态码
来源：http://hz.xinyue.icu/gtnngoeeqt.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ppjwa.cn/gtkjdyexhz.html

[R31] 局部变量
来源：http://hz.hnxiangtu.top/gtwjbmjknb.html

f() { local x=1; echo "$x"; }
来源：http://hz.jianghu66.top/gtqsxveapq.html

[R32] 参数个数校验
来源：http://hz.ydzc1.top/gtqlnwjzls.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.fzhhl.top/gturvhngdu.html

[R33] 捕获错误并提示行号
来源：http://hz.xinyue.icu/gtzorjkvcp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xziqi.cn/gtlukerbgp.html

[R34] 退出时清理
来源：http://hz.wangdashe.top/gtgwaidufu.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinghuilouyu.cn/gtbacffuxf.html

[R35] 后台执行并等待
来源：http://hz.quarkkingdee.top/gtzclpbqqb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yonumen.top/gtoipcxmvb.html

[R36] 并发执行多个任务
来源：http://hz.hongshengwenyu.top/gtiglapwmz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hammf.cn/gtlogjppji.html

[R37] 把输出赋给变量
来源：http://hz.316326.xyz/gtpypnxupm.html

files=$(ls -1)
来源：http://hz.gaohongyu789.top/gtqlohfdvz.html

[R38] 管道串联
来源：http://hz.xuetiantiany.cn/gtyhchicxe.html

cat a.txt | grep -i error | wc -l
来源：http://hz.snrcjt.cn/gtklhzaxej.html

[R39] 重定向标准输出与错误
来源：http://hz.jinqigufen.top/gtpbvlcemf.html

cmd > out.log 2>&1
来源：http://hz.zhaomingkeji.xyz/gtaprviumv.html

[R40] 追加写日志
来源：http://hz.tian-w.cn/gtmqromcyk.html

echo "log" >> out.log
来源：http://hz.birdmap.top/gtjjfbjimq.html

[R41] 丢弃输出
来源：http://hz.ywan-chungtsiang.top/gttvqljjbs.html

cmd >/dev/null 2>&1
来源：http://hz.ppjwa.cn/gtojkxwsxn.html

[R42] 输入重定向
来源：http://hz.kuanghao11.cn/gtsznczocx.html

wc -l < a.txt
来源：http://hz.aibaodan.cn/gtsraxaivj.html

[R43] 按名字查找文件
来源：http://hz.yvedp.cn/gticohhmqm.html

find . -name "*.log" -type f
来源：http://hz.zhaomingkeji.xyz/gtlyxnxjvj.html

[R44] 按修改时间查找
来源：http://hz.shuidangran.top/gtinnzdksc.html

find . -mtime -7 -type f
来源：http://hz.zycfv.cn/gtexlffdix.html

[R45] 批量删除
来源：http://hz.jinqigfzy.top/gtuhcbgkrj.html

find . -name "*.tmp" -delete
来源：http://hz.jianghu66.top/gtjfoixwvi.html

[R46] 递归替换文件内容
来源：http://hz.zhoulong.xyz/gtsyyfnhoi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.kuanghao11.cn/gtkudqscxy.html

[R47] sed 单行替换
来源：http://hz.quarkkingdee.top/gtlbypklpj.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yuxming.cn/gtiqamnvth.html

[R48] awk 取指定列
来源：http://hz.yanxiufei.cn/gtrmhepetv.html

awk '{print $1, $3}' a.txt
来源：http://hz.aibaodan.cn/gtigqfduas.html

[R49] awk 带条件
来源：http://hz.zhijiandao.cn/gtekkjvooz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cdnleiting.top/gtuzlunrho.html

[R50] awk 求和
来源：http://hz.gogol.net.cn/gtkuzslgua.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.pengpengdd.cyou/gtvqxvmojk.html

[R51] 排序去重取前几
来源：http://hz.pengpengdd.cyou/gtgtmpycid.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zycfv.cn/gtdfzeobds.html

[R52] 统计行数
来源：http://hz.jianghu66.top/gtzyitohgi.html

wc -l a.txt
来源：http://hz.9152youxi.cn/gtlywvlzrg.html

[R53] 查看文件头与实时尾
来源：http://hz.tanke756.top/gtwlgfnsxg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.guannengcc.top/gttjxrqwdj.html

[R54] 比较两个文件
来源：http://hz.havefunace.top/gtndhlqqdb.html

diff a.txt b.txt
来源：http://hz.yuanzhike.top/gtykvqmhqs.html

[R55] 压缩与解压
来源：http://hz.aizwys.cn/gtzorwvqup.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.vqdsnc.cn/gthpsnuhfd.html

[R56] 远程拷贝
来源：http://hz.dashuyun.cn/gtzcqpvuto.html

scp file user@host:/path/
来源：http://hz.jinqigfzy.top/gtjojyfxop.html

[R57] 远程执行命令
来源：http://hz.pycfn.com/gtvrrynrfm.html

ssh user@host 'uptime'
来源：http://hz.tianlin.xyz/gtvtoeohbf.html

[R58] 下载文件
来源：http://hz.jinqigfzy.top/gtigzwuzwl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jyoumei.cn/gtcsbjqvzt.html

[R59] 发 POST JSON
来源：http://hz.zhengqikj.top/gtzopeixpu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinghuilouyu.cn/gtiiuulqzv.html

[R60] 只看 HTTP 状态码
来源：http://hz.0kj1m.cn/gtdbfgpcjb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xylfe.cn/gttbyjoizf.html

[R61] 磁盘占用
来源：http://hz.sufxvd.cn/gtqrrpmvhs.html

df -h;  du -sh *
来源：http://hz.cucudq.cn/gtvwmvitut.html

[R62] 找最占空间的文件
来源：http://hz.chenlongwang.top/gtzsuedypz.html

du -ah . | sort -rh | head -10
来源：http://hz.yuxming.cn/gtbtpuvejc.html

[R63] 内存与进程
来源：http://hz.cucudq.cn/gtlbwyrlnq.html

free -h;  ps aux | grep nginx
来源：http://hz.hnxiangtu.top/gtvdydtdpw.html

[R64] 结束进程
来源：http://hz.zhijiandao.cn/gtmwovknqz.html

kill -9 $(pgrep -f app.py)
来源：http://hz.316326.xyz/gtbxinhxgw.html

[R65] 查看端口占用
来源：http://hz.shangyingyoupin.top/gtlkadksmk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yongpay.top/gtbxmqsihc.html

[R66] 定时任务
来源：http://hz.hywenlv.cn/gtahzgdyef.html

crontab -e;  crontab -l
来源：http://hz.sysykeji.top/gtgfutvops.html

[R67] 生成随机十六进制串
来源：http://hz.mhx1999.top/gtqrfmbqpk.html

openssl rand -hex 16
来源：http://hz.snrcjt.cn/gtbrcwfixx.html

[R68] 计算文件校验值
来源：http://hz.shanyushiyangkeji.top/gtvibwdhov.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zdqjudy.top/gtrmlxvobb.html

[R69] 生成随机密码
来源：http://hz.hnxiangtu.top/gtabtoacpo.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhengqikj.top/gtoeedgzub.html

[R70] 时间戳与互转
来源：http://hz.fzhhl.top/gtitlwywgy.html

date +%s;  date -d @1700000000
来源：http://hz.jinqigfzy.top/gtftekyhrq.html

[R71] 日期格式化
来源：http://hz.zhengqikj.top/gtahttulfa.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.dianchejie.cn/gtwyeabgeo.html

[R72] 等待端口就绪
来源：http://hz.smart0.xyz/gtaoowgvnp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ydjk.org.cn/gtcnfsgkjc.html

[R73] 分割大日志
来源：http://hz.zhijiandao.cn/gtruaqzjcu.html

split -l 1000 big.log part_
来源：http://hz.shanyushiyangkeji.top/gtexqgutce.html

[R74] 批量重命名
来源：http://hz.dashuyun.cn/gtbgwfpmbb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yj202588.top/gtvjtuoato.html

[R75] 导出环境变量
来源：http://hz.ivvv.top/gtcoxztntg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.fzhhl.top/gtzefrsdeu.html

[R76] 使用临时文件
来源：http://hz.quarkkingdee.top/gtjtxqlwoj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.birdmap.top/gtedqbzngp.html

[R77] 读取用户输入
来源：http://hz.yueranfly.top/gtnrefyceh.html

read -rp "请输入: " ans
来源：http://hz.ppjwa.cn/gtowbvvylc.html

[R78] 交互式菜单
来源：http://hz.52xcode.cn/gtwfpdaafg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shanyushiyangkeji.top/gtmzhmggcc.html

[R79] 解析命令行选项
来源：http://hz.jlsjyb.cn/gtjrsbxjru.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yongpay.top/gthjtyktpy.html

[R80] 查看脚本执行耗时
来源：http://hz.zhiwuduotai.top/gtpscwuexh.html

time ./run.sh
来源：http://hz.hammf.cn/gtievdggoo.html

================================================================================
来源：http://hz.chenlongwang.top/gtzoydavby.html

S. C / C++ 专题
来源：http://hz.zycfv.cn/gtduhwbyzt.html

================================================================================
来源：http://hz.yj20258888.top/gtvgxcipmt.html

[S01] C：Hello World
来源：http://hz.shzxlz.cn/gtgehxpqjk.html

#include <stdio.h>
来源：http://hz.gotoacloud.top/gtkfoingol.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jinyuanbaomall.cn/gtlzkfursl.html

[S02] C：变量与格式化输出
来源：http://hz.havefunace.top/gtlpuygjkn.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhijiandao.cn/gtwojjtsby.html

[S03] C：读入整数
来源：http://hz.shanyushiyangtech.top/gtamajvqwj.html

int x; scanf("%d", &x);
来源：http://hz.zycfv.cn/gtntpbyvjn.html

[S04] C：字符串复制
来源：http://hz.yueranfly.top/gtvbsgfnut.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.smart0.xyz/gtkatfamuc.html

[S05] C：字符串长度
来源：http://hz.ivvv.top/gtiwdocgfh.html

strlen(s)
来源：http://hz.yj20258888.top/gtvcqeogmn.html

[S06] C：字符串比较
来源：http://hz.yj20258.top/gtxlcgxsns.html

strcmp(a, b) == 0
来源：http://hz.gogol.net.cn/gtdrajwnkt.html

[S07] C：数组遍历求和
来源：http://hz.nanxinkj.top/gtknqkpzxk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.wangshuangyany.cn/gthdtneool.html

[S08] C：动态内存分配与释放
来源：http://hz.xylfe.cn/gttjpoaiff.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yuanzhike.top/gtaxbqtzzd.html

[S09] C：结构体定义与初始化
来源：http://hz.nanxinkj.top/gtbyaaswhv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.birdmap.top/gtgpttozph.html

[S10] C：指针与解引用
来源：http://hz.ybcxt.top/gtdcoshqoa.html

int *p = &a;  *p = 5;
来源：http://hz.chenlongwang.top/gtrltqrpwp.html

[S11] C：逐行读文件
来源：http://hz.feifeiyinyue.top/gtsxzaysgt.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yongpay.top/gtqswhxouz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shangyingyoupin.top/gtfrmmompz.html

fclose(f);
来源：http://hz.guannengcc.top/gtbjbqzsix.html

[S12] C：写文件
来源：http://hz.zhaomingkeji.xyz/gthuysffnw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ywan-chungtsiang.top/gtjzhswwhu.html

[S13] C：宏定义
来源：http://hz.fengsongda.top/gtjpxgcdvf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.havefunace.top/gtshwnmgvp.html

[S14] C：枚举
来源：http://hz.chenzaomai.com/gtdpejxaxv.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.gaohongyu789.top/gtbgwtnqbo.html

[S15] C：类型转换
来源：http://hz.guowangkeji.top/gthgzyvhvy.html

(double) a / b
来源：http://hz.yj202588.top/gtaeldxzhi.html

[S16] C：位操作置位
来源：http://hz.hnxiangtu.top/gtxsuonsam.html

x |= (1 << 3);
来源：http://hz.nanxinkj.top/gtaewafdon.html

[S17] C：安全拼接字符串
来源：http://hz.nanxuanxn.top/gtvntqzzot.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.pycfn.com/gtummhkwpl.html

[S18] C：命令行参数
来源：http://hz.52xcode.cn/gtgdgurnii.html

int main(int argc, char **argv)
来源：http://hz.daria6918.cn/gtqbzelsah.html

[S19] C：快速排序
来源：http://hz.daxiang520.top/gttluhxoev.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhixingplan.top/gtagnickej.html

[S20] C：二分查找
来源：http://hz.chenlongwang.top/gtxjopxxic.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.wangdashe.top/gtsxnphrwb.html

[S21] C：字符类别判断
来源：http://hz.cqqwz.cn/gtqfytchev.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.mhx1999.top/gtleyfqgrg.html

[S22] C：字符串转数字
来源：http://hz.kuanghao11.cn/gthqogewuk.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xinyue.icu/gtwhzcepqi.html

[S23] C：随机数
来源：http://hz.zhongyouzk.top/gttjzzfbcd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.aibaodan.cn/gtmmmyjogi.html

[S24] C：获取本地时间
来源：http://hz.pengpengdd.cyou/gtwwarfjtt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yongpay.top/gtzgteaqkq.html

[S25] C：内存拷贝
来源：http://hz.zhixingplan.top/gtpbgpsvau.html

memcpy(dst, src, n);
来源：http://hz.yj20258.top/gtfdyinnfb.html

[S26] C：内存清零
来源：http://hz.chenlongwang.top/gtdmgseymi.html

memset(a, 0, sizeof a);
来源：http://hz.gogol.net.cn/gtrrwwkcgo.html

[S27] C：定义常量
来源：http://hz.52xcode.cn/gttilwtxlm.html

const double PI = 3.14159;
来源：http://hz.zhijiandao.cn/gtxfqofowq.html

[S28] C：静态变量
来源：http://hz.fzhhl.top/gtaaqparaf.html

static int counter = 0;
来源：http://hz.wangdashe.top/gtujwdkgiz.html

[S29] C：变参函数
来源：http://hz.gotoacloud.top/gtovfjivhi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yueranfly.top/gtvsymjnxh.html

[S30] C：头文件保护
来源：http://hz.yj20258.top/gtrrzfdkjw.html

#ifndef X_H
来源：http://hz.yueranfly.top/gtuhjwhwzv.html

#define X_H
来源：http://hz.haohaochexian.top/gtgrdqmhuf.html

#endif
来源：http://hz.yuxming.cn/gtaxidiadj.html

[S31] C++：Hello World
来源：http://hz.pycfn.com/gtjetkxfiv.html

#include <iostream>
来源：http://hz.daxiang520.top/gtkzzrlgwg.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.wangdashe.top/gtgvdorxce.html

[S32] C++：字符串
来源：http://hz.zdqjudy.top/gtbfjfxndx.html

std::string s = "hi";  s += "!";
来源：http://hz.cheryme.top/gthhiwxwfl.html

[S33] C++：vector 增删
来源：http://hz.jiagoushi.top/gtiwqcnkin.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.316326.xyz/gtshgrmove.html

[S34] C++：遍历 vector
来源：http://hz.gotoacloud.top/gteaklgcbv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ydzc1.top/gtwazsyqkx.html

[S35] C++：map
来源：http://hz.yj20258.top/gtyhumosrt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tianlin.xyz/gteofjsmjt.html

[S36] C++：unordered_map
来源：http://hz.hywenlv.cn/gtanlosqsa.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gaohongyu789.top/gtbwpwchhp.html

[S37] C++：set
来源：http://hz.aizwys.cn/gtqzjychbq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.fengsongda.top/gtzgsrdcgx.html

[S38] C++：排序
来源：http://hz.c1oappe.top/gthqutpcmj.html

std::sort(v.begin(), v.end());
来源：http://hz.tanke756.top/gtuxraipbm.html

[S39] C++：自定义比较器排序
来源：http://hz.zdqjudy.top/gtnkkakujm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.xuanzx.com/gtximsrmqn.html

[S40] C++：查找元素
来源：http://hz.cqqwz.cn/gtdefpxytx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.52xcode.cn/gtlpbuzvrc.html

[S41] C++：类与构造函数
来源：http://hz.jinghuilouyu.cn/gtcfmmmezj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.chenlongwang.top/gtoaxlpnhp.html

[S42] C++：继承与虚函数
来源：http://hz.dianchejie.cn/gtzrdbrqhe.html

class B : public Base { public: void f() override {} };
来源：http://hz.jinghuilouyu.cn/gtioszoftj.html

[S43] C++：智能指针
来源：http://hz.ydjk.org.cn/gtskqtgxfk.html

auto p = std::make_unique<int>(5);
来源：http://hz.sweek.top/gtotcebtvs.html

[S44] C++：引用传参
来源：http://hz.feifeiyinyue.top/gtpkoxwnbx.html

void inc(int &x) { ++x; }
来源：http://hz.ppjwa.cn/gtvwpncolx.html

[S45] C++：lambda
来源：http://hz.aibaodan.cn/gtqtzagqus.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ywan-chungtsiang.top/gtxgwdrsyy.html

[S46] C++：函数模板
来源：http://hz.zycfv.cn/gtzsggvqen.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ybcxt.top/gthxgnjsrx.html

[S47] C++：结构化绑定遍历
来源：http://hz.haohaochexian.top/gtcldclnet.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ppjwa.cn/gttkivoqzz.html

[S48] C++：逐行读文件
来源：http://hz.cdnleiting.top/gtxzekntcm.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.cqqwz.cn/gtpgxpvoff.html

while (std::getline(in, line)) { }
来源：http://hz.yuxming.cn/gtjtvrkvfm.html

[S49] C++：写文件
来源：http://hz.jqgufenzy.top/gtwuofhkxf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.0kj1m.cn/gtsenpavjo.html

[S50] C++：格式化数字
来源：http://hz.zhijiandao.cn/gtbtrslwek.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.gzhubu.top/gtqydikqia.html

[S51] C++：显式类型转换
来源：http://hz.zhijiandao.cn/gtilqgkuxi.html

static_cast<double>(a) / b
来源：http://hz.316326.xyz/gtskzlbrhw.html

[S52] C++：const 与 noexcept
来源：http://hz.xziqi.cn/gtzfjderdo.html

int size() const noexcept { return n_; }
来源：http://hz.yanxiufei.cn/gtrcjhoycj.html

[S53] C++：移动语义
来源：http://hz.xingfuxueyuan.xyz/gtrkfkryen.html

std::vector<int> w = std::move(v);
来源：http://hz.zhijiandao.cn/gtnnxetxre.html

[S54] C++：异常处理
来源：http://hz.tianlin.xyz/gtlwqthrdl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cqqwz.cn/gtgbvrnhyg.html

[S55] C++：结构化绑定
来源：http://hz.zhaomingkeji.xyz/gtbkcqowfw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yueranfly.top/gttrezwvcw.html

[S56] C++：optional
来源：http://hz.yuxming.cn/gtdfnuruvj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jlsjyb.cn/gthfdaurkw.html

[S57] C++：编译期常量
来源：http://hz.jinyuanbaomall.cn/gtrzpfrmuo.html

constexpr int N = 10;
来源：http://hz.cdnleiting.top/gtcbqpnzov.html

[S58] C++：命名空间
来源：http://hz.zhengqikj.top/gtrsbndrln.html

namespace ns { int f() { return 1; } }
来源：http://hz.yongpay.top/gtwsaspacr.html

[S59] C++：静态断言
来源：http://hz.sysykeji.top/gtbygomkfc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xuanzx.com/gtkdvmwvrs.html

[S60] C++：遍历并删除元素
来源：http://hz.sysykeji.top/gtouzhjqvh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.sweek.top/gtuvnzbqqc.html

================================================================================
来源：http://hz.hywenlv.cn/gtxjngccgo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sysykeji.top/gtemqvtikc.html

================================================================================
来源：http://hz.yonumen.top/gtrqmoinpl.html


<!-- 参考信息 -->