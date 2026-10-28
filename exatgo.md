代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.pengpengdd.cyou/gtyzbtdtbl.html

[R10] 正则匹配
来源：http://hz.zhengqikj.top/gtsyvrjwww.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.iojbl.cn/gtjpxsoblw.html

[R11] case 多分支
来源：http://hz.zhengqikj.top/gtkmrpurcm.html

case "$1" in
来源：http://hz.dashuyun.cn/gtxrpfemzg.html

start) echo "启动" ;;
来源：http://hz.daxiang520.top/gtowcsgxtn.html

stop)  echo "停止" ;;
来源：http://hz.chenjidiqi.icu/gtbhkcyusg.html

*)     echo "未知命令" ;;
来源：http://hz.ydzc1.top/gtbcthpvtv.html

esac
来源：http://hz.wangdashe.top/gtgasogqxh.html

[R12] for 遍历文件
来源：http://hz.guannengcc.top/gteafpplul.html

for f in *.txt; do echo "$f"; done
来源：http://hz.wangdashe.top/gtrvteqkeo.html

[R13] for 计数循环
来源：http://hz.cashguo.top/gtlfvvzrob.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.vqdsnc.cn/gtetvkvnma.html

[R14] C 风格 for
来源：http://hz.havefunace.top/gtzzhfzitt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jinqigfzy.top/gtwjgoeqpj.html

[R15] while 逐行读文件
来源：http://hz.wangshuangyany.cn/gtsjblhbtc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.dianchejie.cn/gtdltlspfv.html

[R16] until 等待条件
来源：http://hz.xuetiantiany.cn/gtlyymjeix.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.tianlin.xyz/gtkkjvrvtt.html

[R17] 数组定义与取值
来源：http://hz.yuanzhike.top/gttajgjnne.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cdnleiting.top/gthkmelnjv.html

[R18] 遍历数组
来源：http://hz.sweek.top/gtofofcxfc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.redwolf501.top/gtftsojebt.html

[R19] 数组长度
来源：http://hz.ehwqpu.com/gtukvwyoxz.html

echo "${#arr[@]}"
来源：http://hz.guowangkeji.top/gtacxmpttz.html

[R20] 关联数组（字典）
来源：http://hz.haohaochexian.top/gttsnzzssy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.tianlin.xyz/gtkuhvdbrd.html

[R21] 字符串长度
来源：http://hz.gaohongyu789.top/gtcdeckdtq.html

echo "${#s}"
来源：http://hz.chenzaomai.com/gtbfhcdeet.html

[R22] 截取子串
来源：http://hz.gotoacloud.top/gtnvpuecji.html

echo "${s:0:5}"
来源：http://hz.jyoumei.cn/gtutbezujr.html

[R23] 字符串替换
来源：http://hz.nanxinkj.top/gtcxnjkour.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sufxvd.cn/gtrnngyaxv.html

[R24] 大小写转换
来源：http://hz.feifeiyinyue.top/gtvgxokkii.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.nwbrower.top/gtrmhehnpt.html

[R25] 去后缀 / 去前缀
来源：http://hz.ybcxt.top/gtdiqzfzxd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhixingplan.top/gtikfttdjp.html

[R26] 命令替换
来源：http://hz.jiagoushi.top/gtspxomasz.html

now=$(date +%F); echo "$now"
来源：http://hz.yuxming.cn/gtnbxsgtga.html

[R27] 算术展开
来源：http://hz.zhiwuduotai.top/gtmjohwfzo.html

echo $((1 + 2 * 3))
来源：http://hz.gotoacloud.top/gtxaearquq.html

[R28] 浮点运算
来源：http://hz.fzhhl.top/gtnkofhucm.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhengqikj.top/gtaonxxajd.html

[R29] 定义函数
来源：http://hz.gaohongyu789.top/gtkfpptqow.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yj202588.top/gtuelxcbjl.html

[R30] 函数返回状态码
来源：http://hz.ppjwa.cn/gtdxmrjbnk.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.nanxinkj.top/gtwsrlveaa.html

[R31] 局部变量
来源：http://hz.nwbrower.top/gthhtucxqo.html

f() { local x=1; echo "$x"; }
来源：http://hz.sxryk.cn/gttejiaafy.html

[R32] 参数个数校验
来源：http://hz.xinyue.icu/gtmgecizfo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.sufxvd.cn/gtinbuixxx.html

[R33] 捕获错误并提示行号
来源：http://hz.chenzaomai.com/gthqqhllaz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yj20258888.top/gtwmrwrpsx.html

[R34] 退出时清理
来源：http://hz.vqdsnc.cn/gtchdxnznk.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenlongwang.top/gtbkxypujc.html

[R35] 后台执行并等待
来源：http://hz.nanxinkj.top/gtyrxgwhvl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.9152youxi.cn/gtyggamvsc.html

[R36] 并发执行多个任务
来源：http://hz.zhongyouzk.top/gttpctovoy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.svipenyu.cn/gtnnjllnup.html

[R37] 把输出赋给变量
来源：http://hz.sysykeji.top/gtngkakyfr.html

files=$(ls -1)
来源：http://hz.gaohongyu789.top/gtbjtuikam.html

[R38] 管道串联
来源：http://hz.havefunace.top/gtlprljpio.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yj20258888.top/gtjwfmqgab.html

[R39] 重定向标准输出与错误
来源：http://hz.yj202588.top/gtnowermhh.html

cmd > out.log 2>&1
来源：http://hz.cqqwz.cn/gtksozrjjj.html

[R40] 追加写日志
来源：http://hz.chenjidiqi.icu/gtufyhseuz.html

echo "log" >> out.log
来源：http://hz.zdqjudy.top/gtxzmzgxdm.html

[R41] 丢弃输出
来源：http://hz.guowangkeji.top/gtssdmzqlc.html

cmd >/dev/null 2>&1
来源：http://hz.yj20258.top/gtybnxjxyo.html

[R42] 输入重定向
来源：http://hz.cqqwz.cn/gtpjovtctf.html

wc -l < a.txt
来源：http://hz.shangyingyoupin.top/gtsynrxrxf.html

[R43] 按名字查找文件
来源：http://hz.yanxiufei.cn/gtzyropjxj.html

find . -name "*.log" -type f
来源：http://hz.zhaomingkeji.xyz/gthjtejkmo.html

[R44] 按修改时间查找
来源：http://hz.zycfv.cn/gtjmsnghqx.html

find . -mtime -7 -type f
来源：http://hz.jianghu66.top/gtvuhlnbhw.html

[R45] 批量删除
来源：http://hz.xuanzx.com/gtrrqqysja.html

find . -name "*.tmp" -delete
来源：http://hz.jqgfzy.top/gtvrbrftxd.html

[R46] 递归替换文件内容
来源：http://hz.jinghuilouyu.cn/gtjshqxlwb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yangfankeji.com/gtquwjtxzn.html

[R47] sed 单行替换
来源：http://hz.yuxming.cn/gtcfxkuojh.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.cdnleiting.top/gtxpnoneai.html

[R48] awk 取指定列
来源：http://hz.xuetiantiany.cn/gtivuauuva.html

awk '{print $1, $3}' a.txt
来源：http://hz.ivvv.top/gttlwauuqs.html

[R49] awk 带条件
来源：http://hz.tian-w.cn/gtcwnyqygm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.gzhubu.top/gtgfcmibge.html

[R50] awk 求和
来源：http://hz.nanxinkj.top/gteqkvjrmg.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yangfankeji.com/gtwwewlldk.html

[R51] 排序去重取前几
来源：http://hz.sxryk.cn/gtaehorzkp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.birdmap.top/gtnuaalwym.html

[R52] 统计行数
来源：http://hz.chenlongwang.top/gtgvoljukx.html

wc -l a.txt
来源：http://hz.sxryk.cn/gtmmstzvzi.html

[R53] 查看文件头与实时尾
来源：http://hz.cheryme.top/gtufubluzr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.chenjidiqi.icu/gtkccijijb.html

[R54] 比较两个文件
来源：http://hz.fzhhl.top/gtzbnpsnwm.html

diff a.txt b.txt
来源：http://hz.cheryme.top/gtjgyhbeoa.html

[R55] 压缩与解压
来源：http://hz.tian-w.cn/gtnainumwh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hywenlv.cn/gtwnuqimqj.html

[R56] 远程拷贝
来源：http://hz.yongpay.top/gtezqhaevt.html

scp file user@host:/path/
来源：http://hz.pycfn.com/gtcbxdtziu.html

[R57] 远程执行命令
来源：http://hz.hywenlv.cn/gttbcjagxs.html

ssh user@host 'uptime'
来源：http://hz.guannengcc.top/gtejssiqzr.html

[R58] 下载文件
来源：http://hz.dashuyun.cn/gtpiweiqwf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.wangshuangyany.cn/gtulibuzdm.html

[R59] 发 POST JSON
来源：http://hz.meibo888.top/gtmrwupexx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yongpay.top/gtezbjoyzm.html

[R60] 只看 HTTP 状态码
来源：http://hz.fengsongda.top/gtupaafmvk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shangyingyoupin.top/gtmgwyjfwr.html

[R61] 磁盘占用
来源：http://hz.yueranfly.top/gtrbswoowf.html

df -h;  du -sh *
来源：http://hz.birdmap.top/gtfunpdawx.html

[R62] 找最占空间的文件
来源：http://hz.jqgufenzy.top/gtutceuvft.html

du -ah . | sort -rh | head -10
来源：http://hz.hnqzz.top/gtqwhghifg.html

[R63] 内存与进程
来源：http://hz.tanke756.top/gtplipdfqy.html

free -h;  ps aux | grep nginx
来源：http://hz.hfpthk.cn/gtayphqedm.html

[R64] 结束进程
来源：http://hz.daxiang520.top/gttlneytyr.html

kill -9 $(pgrep -f app.py)
来源：http://hz.pengpengdd.cyou/gtvcmbeecs.html

[R65] 查看端口占用
来源：http://hz.cashguo.top/gtejsdenhq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.nanxinkj.top/gtfgnrbhfs.html

[R66] 定时任务
来源：http://hz.pengpengdd.cyou/gtsgkpewou.html

crontab -e;  crontab -l
来源：http://hz.cucudq.cn/gtdoedazgo.html

[R67] 生成随机十六进制串
来源：http://hz.haohaochexian.top/gtngriiumu.html

openssl rand -hex 16
来源：http://hz.yuxming.cn/gtryrvtypm.html

[R68] 计算文件校验值
来源：http://hz.yj20258.top/gtvbhjrcln.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yj20258.top/gtajpdqmmc.html

[R69] 生成随机密码
来源：http://hz.yanxiufei.cn/gtcjwiuvsh.html

head -c 16 /dev/urandom | base64
来源：http://hz.hnqzz.top/gtdlqsvznf.html

[R70] 时间戳与互转
来源：http://hz.fzhhl.top/gtqwfvwwff.html

date +%s;  date -d @1700000000
来源：http://hz.havefunace.top/gtwhyifscr.html

[R71] 日期格式化
来源：http://hz.xinyue.icu/gtydqjiead.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yj20258888.top/gtcsekqkuz.html

[R72] 等待端口就绪
来源：http://hz.hammf.cn/gterlrbenh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.guowangkeji.top/gtyjtnrppd.html

[R73] 分割大日志
来源：http://hz.smart0.xyz/gtnbevjftb.html

split -l 1000 big.log part_
来源：http://hz.52xcode.cn/gtpyykgglw.html

[R74] 批量重命名
来源：http://hz.yangfankeji.com/gtsgepmnnw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.gogol.net.cn/gtdshjkfls.html

[R75] 导出环境变量
来源：http://hz.xuetiantiany.cn/gtathsqqcw.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.316326.xyz/gtkboooqew.html

[R76] 使用临时文件
来源：http://hz.zdqjudy.top/gttgbyaoan.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cucudq.cn/gtxomoponj.html

[R77] 读取用户输入
来源：http://hz.c1oappe.top/gtyrevkcoz.html

read -rp "请输入: " ans
来源：http://hz.snrcjt.cn/gtueuctbbi.html

[R78] 交互式菜单
来源：http://hz.shuidangran.top/gtqigqydmv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xuetiantiany.cn/gtlqunmizf.html

[R79] 解析命令行选项
来源：http://hz.316326.xyz/gtqjvnfnju.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shanyushiyangtech.top/gtkpgkkpbg.html

[R80] 查看脚本执行耗时
来源：http://hz.wangshuangyany.cn/gtxhhyxpfp.html

time ./run.sh
来源：http://hz.aibaodan.cn/gtoagheycr.html

================================================================================
来源：http://hz.xziqi.cn/gtcmpigmav.html

S. C / C++ 专题
来源：http://hz.ybcxt.top/gtbkzurxfm.html

================================================================================
来源：http://hz.ybcxt.top/gtrfsmpcva.html

[S01] C：Hello World
来源：http://hz.bjfxy.top/gtqsrutgph.html

#include <stdio.h>
来源：http://hz.sxryk.cn/gtoewvxpcr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jlsjyb.cn/gtrbxmjgnx.html

[S02] C：变量与格式化输出
来源：http://hz.jinyuanbaomall.cn/gtgeutajrv.html

int a = 10; printf("%d\n", a);
来源：http://hz.sweek.top/gtrbpkeatf.html

[S03] C：读入整数
来源：http://hz.ivvv.top/gtfdtphqni.html

int x; scanf("%d", &x);
来源：http://hz.zhaomingkeji.xyz/gtbifduvwf.html

[S04] C：字符串复制
来源：http://hz.tianlin.xyz/gtpvneuhwj.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinghuilouyu.cn/gtjnuirscs.html

[S05] C：字符串长度
来源：http://hz.gzhubu.top/gtiqqraggg.html

strlen(s)
来源：http://hz.sxryk.cn/gtqezaqjbb.html

[S06] C：字符串比较
来源：http://hz.nanxuanxn.top/gtqqdhympt.html

strcmp(a, b) == 0
来源：http://hz.sufxvd.cn/gtfcdnislg.html

[S07] C：数组遍历求和
来源：http://hz.yvedp.cn/gtlljtkzvm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zycfv.cn/gtrwvhjlut.html

[S08] C：动态内存分配与释放
来源：http://hz.tanke756.top/gtqsyhpdor.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.vqdsnc.cn/gtofmimksg.html

[S09] C：结构体定义与初始化
来源：http://hz.nanxinkj.top/gthwtygkws.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.tanke756.top/gtdosvkfap.html

[S10] C：指针与解引用
来源：http://hz.dianchejie.cn/gtcpqmxint.html

int *p = &a;  *p = 5;
来源：http://hz.feifeiyinyue.top/gtnnjymmka.html

[S11] C：逐行读文件
来源：http://hz.dianchejie.cn/gtybygipyt.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.kuanghao11.cn/gtbpohcnpk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yonumen.top/gtxccwhacd.html

fclose(f);
来源：http://hz.9152youxi.cn/gtkhgwsydx.html

[S12] C：写文件
来源：http://hz.cucudq.cn/gtiudhkuow.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.0kj1m.cn/gtczgoecqm.html

[S13] C：宏定义
来源：http://hz.vqdsnc.cn/gtbvkghqmz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.0kj1m.cn/gtathvpnrr.html

[S14] C：枚举
来源：http://hz.redwolf501.top/gtevuxxfmu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.chenjidiqi.icu/gtmhpbrgiq.html

[S15] C：类型转换
来源：http://hz.zhongyouzk.top/gtmrxkxsfi.html

(double) a / b
来源：http://hz.zhaomingkeji.xyz/gtoanbwxyv.html

[S16] C：位操作置位
来源：http://hz.zhixingplan.top/gtrttliydn.html

x |= (1 << 3);
来源：http://hz.yuxming.cn/gtwmhmvcmc.html

[S17] C：安全拼接字符串
来源：http://hz.zdqjudy.top/gtxspatzgl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ybcxt.top/gtxhwkqdcs.html

[S18] C：命令行参数
来源：http://hz.yongpay.top/gtmzpejzih.html

int main(int argc, char **argv)
来源：http://hz.cucudq.cn/gtqruedvmb.html

[S19] C：快速排序
来源：http://hz.haohaochexian.top/gtireduslj.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhijiandao.cn/gtxdxpdsbt.html

[S20] C：二分查找
来源：http://hz.cashguo.top/gtoinunyub.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cheryme.top/gtgewntrnv.html

[S21] C：字符类别判断
来源：http://hz.zhiwuduotai.top/gtskplyxes.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhaomingkeji.xyz/gtywsgcjwn.html

[S22] C：字符串转数字
来源：http://hz.cqqwz.cn/gtuipyodpy.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.nanxinkj.top/gtlfigkhnk.html

[S23] C：随机数
来源：http://hz.shangyingyoupin.top/gtddgyucro.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhaomingkeji.xyz/gtgzcwvmgd.html

[S24] C：获取本地时间
来源：http://hz.ydzc1.top/gtdmuovyie.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shuidangran.top/gthywkwuux.html

[S25] C：内存拷贝
来源：http://hz.nanxinkj.top/gtcoagatjk.html

memcpy(dst, src, n);
来源：http://hz.tianlin.xyz/gtzpgomjgf.html

[S26] C：内存清零
来源：http://hz.quarkkingdee.top/gtpmzbotlb.html

memset(a, 0, sizeof a);
来源：http://hz.aibaodan.cn/gtgspjfsia.html

[S27] C：定义常量
来源：http://hz.yueranfly.top/gtolipnvwl.html

const double PI = 3.14159;
来源：http://hz.nanxuanxn.top/gtbbofzuqb.html

[S28] C：静态变量
来源：http://hz.daria6918.cn/gtsanvqprc.html

static int counter = 0;
来源：http://hz.dashuyun.cn/gtfwfxanpq.html

[S29] C：变参函数
来源：http://hz.shangyingyoupin.top/gtecuaveua.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.guannengcc.top/gtcequaznb.html

[S30] C：头文件保护
来源：http://hz.hnqzz.top/gteimoxndd.html

#ifndef X_H
来源：http://hz.yj202588.top/gtynwewvsp.html

#define X_H
来源：http://hz.daxiang520.top/gtsdhvfgcb.html

#endif
来源：http://hz.gogol.net.cn/gtyfmuobxi.html

[S31] C++：Hello World
来源：http://hz.ydzc1.top/gtnwgyzzjf.html

#include <iostream>
来源：http://hz.guowangkeji.top/gtbvjwphug.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.mhx1999.top/gtqvsmpdea.html

[S32] C++：字符串
来源：http://hz.dashuyun.cn/gtejlvvdrl.html

std::string s = "hi";  s += "!";
来源：http://hz.vqdsnc.cn/gtmimacwpw.html

[S33] C++：vector 增删
来源：http://hz.jiagoushi.top/gtxymarwsh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.tanke756.top/gtlbmqhpno.html

[S34] C++：遍历 vector
来源：http://hz.xuanzx.com/gtlegqzdiw.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cashguo.top/gtlcckcwoa.html

[S35] C++：map
来源：http://hz.hnqzz.top/gtjizznqaa.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenzaomai.com/gtlllvvxih.html

[S36] C++：unordered_map
来源：http://hz.pycfn.com/gtsokzsdqw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.havefunace.top/gtwpcemjss.html

[S37] C++：set
来源：http://hz.52xcode.cn/gtchnxojwp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yvedp.cn/gtwwbtqqkw.html

[S38] C++：排序
来源：http://hz.chenjidiqi.icu/gtlbknzwfh.html

std::sort(v.begin(), v.end());
来源：http://hz.ydjk.org.cn/gtnwedenzy.html

[S39] C++：自定义比较器排序
来源：http://hz.yuanzhike.top/gtfltnltpz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.svipenyu.cn/gtzyegwolg.html

[S40] C++：查找元素
来源：http://hz.snrcjt.cn/gtdshssgrg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shangyingyoupin.top/gtfmqljzzh.html

[S41] C++：类与构造函数
来源：http://hz.redwolf501.top/gtvbhtrgkk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.snrcjt.cn/gtdjzsvjlq.html

[S42] C++：继承与虚函数
来源：http://hz.hammf.cn/gtydhkckce.html

class B : public Base { public: void f() override {} };
来源：http://hz.tanke756.top/gtpefhuefv.html

[S43] C++：智能指针
来源：http://hz.zhaomingkeji.xyz/gtbaevcefd.html

auto p = std::make_unique<int>(5);
来源：http://hz.dianchejie.cn/gtlmzdrvku.html

[S44] C++：引用传参
来源：http://hz.fzhhl.top/gtbezktyrc.html

void inc(int &x) { ++x; }
来源：http://hz.cdnleiting.top/gtjuwixiha.html

[S45] C++：lambda
来源：http://hz.bjfxy.top/gtvxktmhaw.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hywenlv.cn/gtezmcfoqp.html

[S46] C++：函数模板
来源：http://hz.cdnleiting.top/gtidwlfdax.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.gzhubu.top/gtgdeymuut.html

[S47] C++：结构化绑定遍历
来源：http://hz.52xcode.cn/gtkxbhtrzn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.chenjidiqi.icu/gtsjavdsem.html

[S48] C++：逐行读文件
来源：http://hz.yongpay.top/gtyvicygep.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhongyouzk.top/gtsnkdrppq.html

while (std::getline(in, line)) { }
来源：http://hz.feifeiyinyue.top/gtllroqssl.html

[S49] C++：写文件
来源：http://hz.fzhhl.top/gtelichtro.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cheryme.top/gtmyesqbaz.html

[S50] C++：格式化数字
来源：http://hz.xinyue.icu/gtlxlwttea.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.sysykeji.top/gtgpzoybam.html

[S51] C++：显式类型转换
来源：http://hz.ydzc1.top/gtzjrspgow.html

static_cast<double>(a) / b
来源：http://hz.cqqwz.cn/gtgdnlsmew.html

[S52] C++：const 与 noexcept
来源：http://hz.zhoulong.xyz/gtmlpmvpib.html

int size() const noexcept { return n_; }
来源：http://hz.yvedp.cn/gtwwbenaav.html

[S53] C++：移动语义
来源：http://hz.jianghu66.top/gtuljrtaij.html

std::vector<int> w = std::move(v);
来源：http://hz.tian-w.cn/gtegmnials.html

[S54] C++：异常处理
来源：http://hz.xinyue.icu/gtlsxfmsuz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.chenlongwang.top/gtwjhxujwm.html

[S55] C++：结构化绑定
来源：http://hz.ivvv.top/gteiwkssxm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yj202588.top/gtpbtyypvv.html

[S56] C++：optional
来源：http://hz.cqqwz.cn/gtppqwlboo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.dashuyun.cn/gtviaztjsp.html

[S57] C++：编译期常量
来源：http://hz.cdnleiting.top/gtwcfxdoay.html

constexpr int N = 10;
来源：http://hz.gzhubu.top/gtrnnwwatt.html

[S58] C++：命名空间
来源：http://hz.gogol.net.cn/gtpjkcjnay.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhongyouzk.top/gtbxrjhxsn.html

[S59] C++：静态断言
来源：http://hz.tian-w.cn/gtvttqjspp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xziqi.cn/gtsafnwfwo.html

[S60] C++：遍历并删除元素
来源：http://hz.vqdsnc.cn/gtvrthoapk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shanyushiyangkeji.top/gtqnnhfqig.html

================================================================================
来源：http://hz.ehwqpu.com/gtsmfodbzl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hywenlv.cn/gtphhumtac.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtbhsuyttn.html

[T01] Kotlin：Hello World
来源：http://hz.yvedp.cn/gtdffhdfjd.html

println("Hello")
来源：http://hz.yj202588.top/gtbrtktspt.html

[T02] Kotlin：变量
来源：http://hz.bjfxy.top/gtyocgrxvw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.dashuyun.cn/gtmtusbtug.html

[T03] Kotlin：字符串模板
来源：http://hz.zhaomingkeji.xyz/gtolhprmih.html

"值: $b"
来源：http://hz.zhoulong.xyz/gtoavdynyp.html

[T04] Kotlin：空安全
来源：http://hz.xuanzx.com/gtdruiqflm.html

val n: String? = null;  n?.length
来源：http://hz.zdqjudy.top/gtfhknwshy.html

[T05] Kotlin：when 表达式
来源：http://hz.cqqwz.cn/gtyrmkfkvf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hnqzz.top/gtjwpdgame.html

[T06] Kotlin：集合映射
来源：http://hz.yj20258888.top/gtxxxwsiqr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.sxryk.cn/gtngbogkuz.html

[T07] Kotlin：集合过滤
来源：http://hz.ivvv.top/gtymujryou.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.pycfn.com/gtrmlttndv.html

[T08] Kotlin：数据类
来源：http://hz.yanxiufei.cn/gtsuiztobt.html

data class User(val name: String, val age: Int)
来源：http://hz.tanke756.top/gtjurznofq.html

[T09] Kotlin：扩展函数
来源：http://hz.zhengqikj.top/gttrjjyilu.html

fun String.exclaim() = this + "!"
来源：http://hz.zhoulong.xyz/gtsoajroea.html

[T10] Kotlin：默认参数
来源：http://hz.daria6918.cn/gtxmauhzmv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.chenjidiqi.icu/gtzqpkugrv.html


<!-- 参考信息 -->