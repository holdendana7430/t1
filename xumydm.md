代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.tian-w.cn/gthkrxuuzm.html

[R10] 正则匹配
来源：http://hz.aizwys.cn/gttsnvpyte.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yuanzhike.top/gtdtakmjvb.html

[R11] case 多分支
来源：http://hz.andypj.xyz/gtrfusvogr.html

case "$1" in
来源：http://hz.ehwqpu.com/gtxplohryf.html

start) echo "启动" ;;
来源：http://hz.sysykeji.top/gtoxexijas.html

stop)  echo "停止" ;;
来源：http://hz.chenlongwang.top/gtxuomsefn.html

*)     echo "未知命令" ;;
来源：http://hz.daxiang520.top/gtgwdxmerh.html

esac
来源：http://hz.316326.xyz/gtzeqqrnkb.html

[R12] for 遍历文件
来源：http://hz.shuidangran.top/gthogtyqrl.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ywan-chungtsiang.top/gtajiqniro.html

[R13] for 计数循环
来源：http://hz.guannengcc.top/gtzlvomyws.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ydjk.org.cn/gtrnwybwon.html

[R14] C 风格 for
来源：http://hz.jiagoushi.top/gtxazqvbtc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jlsjyb.cn/gtzjpivgrn.html

[R15] while 逐行读文件
来源：http://hz.hysaishi.cn/gtzuyxxdpv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.chenzaomai.com/gtjeuvkuej.html

[R16] until 等待条件
来源：http://hz.kuanghao11.cn/gteffjtmiw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.haohaochexian.top/gthixpycts.html

[R17] 数组定义与取值
来源：http://hz.dashuyun.cn/gttlceyncy.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.gogol.net.cn/gtkelbwhyz.html

[R18] 遍历数组
来源：http://hz.quarkkingdee.top/gtpjdwgkrh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.redwolf501.top/gtkklwiwss.html

[R19] 数组长度
来源：http://hz.kuanghao11.cn/gtrrbjcheg.html

echo "${#arr[@]}"
来源：http://hz.gaohongyu789.top/gtbgcqhzbh.html

[R20] 关联数组（字典）
来源：http://hz.jinghuilouyu.cn/gtvmwyzqox.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hnqzz.top/gtelffmtgf.html

[R21] 字符串长度
来源：http://hz.wangshuangyany.cn/gtmflsfwdy.html

echo "${#s}"
来源：http://hz.shanyushiyangtech.top/gtkxmfhlan.html

[R22] 截取子串
来源：http://hz.jianghu66.top/gtrkwdeeak.html

echo "${s:0:5}"
来源：http://hz.fzhhl.top/gthgpsgqwi.html

[R23] 字符串替换
来源：http://hz.hnqzz.top/gtcdpsexwx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.wangshuangyany.cn/gtumiitvcl.html

[R24] 大小写转换
来源：http://hz.9152youxi.cn/gtleikpqjq.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jyoumei.cn/gtwhptvbko.html

[R25] 去后缀 / 去前缀
来源：http://hz.hnqzz.top/gtkuhehaff.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xingfuxueyuan.xyz/gtqayyvesd.html

[R26] 命令替换
来源：http://hz.sufxvd.cn/gtfubfzokm.html

now=$(date +%F); echo "$now"
来源：http://hz.sufxvd.cn/gtllvzlebl.html

[R27] 算术展开
来源：http://hz.yuxming.cn/gtrlehbmmq.html

echo $((1 + 2 * 3))
来源：http://hz.zhaomingkeji.xyz/gtdubwdjjj.html

[R28] 浮点运算
来源：http://hz.yvedp.cn/gtlogczemq.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhijiandao.cn/gttnywhtbx.html

[R29] 定义函数
来源：http://hz.fzhhl.top/gtbpbkqxdw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zdqjudy.top/gtcpszssau.html

[R30] 函数返回状态码
来源：http://hz.0kj1m.cn/gtrngpbrri.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xuanzx.com/gtolecksfq.html

[R31] 局部变量
来源：http://hz.ydzc1.top/gtnanstmxf.html

f() { local x=1; echo "$x"; }
来源：http://hz.fzhhl.top/gtbagrceff.html

[R32] 参数个数校验
来源：http://hz.zhongyouzk.top/gtilzbperm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shangyingyoupin.top/gtzlevsguj.html

[R33] 捕获错误并提示行号
来源：http://hz.daxiang520.top/gtzthabvfj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.feifeiyinyue.top/gtgflhnvlf.html

[R34] 退出时清理
来源：http://hz.fzhhl.top/gtyqlwzjqf.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yvedp.cn/gtwqdrbcjh.html

[R35] 后台执行并等待
来源：http://hz.jinghuilouyu.cn/gtjtwejigb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xuetiantiany.cn/gtujlfojot.html

[R36] 并发执行多个任务
来源：http://hz.jinyuanbaomall.cn/gtpgvhhzyu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cqqwz.cn/gtzvdbxvaq.html

[R37] 把输出赋给变量
来源：http://hz.cqqwz.cn/gtuqjsaumt.html

files=$(ls -1)
来源：http://hz.jqgufenzy.top/gtivrjohqn.html

[R38] 管道串联
来源：http://hz.hnxiangtu.top/gtxyralpib.html

cat a.txt | grep -i error | wc -l
来源：http://hz.shangyingyoupin.top/gtimgtzdrs.html

[R39] 重定向标准输出与错误
来源：http://hz.aizwys.cn/gtuykrksgm.html

cmd > out.log 2>&1
来源：http://hz.yuxming.cn/gtpmpqpjun.html

[R40] 追加写日志
来源：http://hz.0kj1m.cn/gtwkagadbk.html

echo "log" >> out.log
来源：http://hz.cucudq.cn/gtmwuoobro.html

[R41] 丢弃输出
来源：http://hz.c1oappe.top/gtedadguxo.html

cmd >/dev/null 2>&1
来源：http://hz.zhiwuduotai.top/gtnmvixejv.html

[R42] 输入重定向
来源：http://hz.yj20258.top/gtztwiinih.html

wc -l < a.txt
来源：http://hz.redwolf501.top/gtgqidxiek.html

[R43] 按名字查找文件
来源：http://hz.ehwqpu.com/gtuffcvciu.html

find . -name "*.log" -type f
来源：http://hz.shanyushiyangkeji.top/gtoyxmnxdb.html

[R44] 按修改时间查找
来源：http://hz.fengsongda.top/gtevjjwkim.html

find . -mtime -7 -type f
来源：http://hz.ywan-chungtsiang.top/gtlysoukvy.html

[R45] 批量删除
来源：http://hz.shzxlz.cn/gtpztqnfub.html

find . -name "*.tmp" -delete
来源：http://hz.zhaomingkeji.xyz/gtjqrwixdo.html

[R46] 递归替换文件内容
来源：http://hz.chenzaomai.com/gtllqyzpfa.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.vqdsnc.cn/gtyfktsrow.html

[R47] sed 单行替换
来源：http://hz.sufxvd.cn/gtcxgnjndg.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.andypj.xyz/gtgvxacuws.html

[R48] awk 取指定列
来源：http://hz.nanxinkj.top/gtnwwuvish.html

awk '{print $1, $3}' a.txt
来源：http://hz.xuanzx.com/gtbiwfsmvc.html

[R49] awk 带条件
来源：http://hz.pengpengdd.cyou/gtglqkroel.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.daria6918.cn/gtmmdaggit.html

[R50] awk 求和
来源：http://hz.quarkkingdee.top/gtfgwadmrd.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.snrcjt.cn/gtdewimhyh.html

[R51] 排序去重取前几
来源：http://hz.shuidangran.top/gtwddgmgmd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yonumen.top/gtgknlppkj.html

[R52] 统计行数
来源：http://hz.yvedp.cn/gtvvpgpotr.html

wc -l a.txt
来源：http://hz.snrcjt.cn/gtzzabixtw.html

[R53] 查看文件头与实时尾
来源：http://hz.xylfe.cn/gtzcprumwj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.tian-w.cn/gtzrbelnjl.html

[R54] 比较两个文件
来源：http://hz.pengpengdd.cyou/gtqmlmfuma.html

diff a.txt b.txt
来源：http://hz.yonumen.top/gthcmexysj.html

[R55] 压缩与解压
来源：http://hz.pycfn.com/gtiriyetio.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.pycfn.com/gtflxfxncz.html

[R56] 远程拷贝
来源：http://hz.shzxlz.cn/gtdiairbvd.html

scp file user@host:/path/
来源：http://hz.hnqzz.top/gtprhtgohb.html

[R57] 远程执行命令
来源：http://hz.ywan-chungtsiang.top/gtlhffzfaa.html

ssh user@host 'uptime'
来源：http://hz.xziqi.cn/gtvzfbhemy.html

[R58] 下载文件
来源：http://hz.sxryk.cn/gtruftmgwn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.tianlin.xyz/gtazsyfobs.html

[R59] 发 POST JSON
来源：http://hz.yueranfly.top/gtochsrsgv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.svipenyu.cn/gtlvpczidc.html

[R60] 只看 HTTP 状态码
来源：http://hz.xziqi.cn/gtbytdjvkm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hammf.cn/gtlspkzysq.html

[R61] 磁盘占用
来源：http://hz.hammf.cn/gtptjztrrx.html

df -h;  du -sh *
来源：http://hz.gzhubu.top/gtqeegzxih.html

[R62] 找最占空间的文件
来源：http://hz.cheryme.top/gtofwlssnq.html

du -ah . | sort -rh | head -10
来源：http://hz.gzhubu.top/gtflolnzzt.html

[R63] 内存与进程
来源：http://hz.wangshuangyany.cn/gtvpruiboh.html

free -h;  ps aux | grep nginx
来源：http://hz.chenlongwang.top/gtiyyhcurz.html

[R64] 结束进程
来源：http://hz.jqgfzy.top/gtiysigybd.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ydjk.org.cn/gtilwliyqe.html

[R65] 查看端口占用
来源：http://hz.sweek.top/gtyxkgoqej.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.wangdashe.top/gtprftozlv.html

[R66] 定时任务
来源：http://hz.dianchejie.cn/gtvzdcsizz.html

crontab -e;  crontab -l
来源：http://hz.kuanghao11.cn/gtqtjfvrmx.html

[R67] 生成随机十六进制串
来源：http://hz.havefunace.top/gtxikbheyw.html

openssl rand -hex 16
来源：http://hz.ydzc1.top/gtzgjclmhx.html

[R68] 计算文件校验值
来源：http://hz.ivvv.top/gtlfnvuqdm.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.nanxuanxn.top/gtwazullni.html

[R69] 生成随机密码
来源：http://hz.zhongyouzk.top/gtfvluetpz.html

head -c 16 /dev/urandom | base64
来源：http://hz.sufxvd.cn/gtsqldoupr.html

[R70] 时间戳与互转
来源：http://hz.birdmap.top/gtvnymilpl.html

date +%s;  date -d @1700000000
来源：http://hz.zhaomingkeji.xyz/gtzyikzmnj.html

[R71] 日期格式化
来源：http://hz.nanxinkj.top/gtmpgphsvh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shangyingyoupin.top/gtqugcgoly.html

[R72] 等待端口就绪
来源：http://hz.xinyue.icu/gtofpothfc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.sxryk.cn/gtwmityjsl.html

[R73] 分割大日志
来源：http://hz.dianchejie.cn/gtbjukbnjb.html

split -l 1000 big.log part_
来源：http://hz.pengpengdd.cyou/gtxfdfcffh.html

[R74] 批量重命名
来源：http://hz.yangfankeji.com/gtszwtvigh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.gaohongyu789.top/gtmvanrdrb.html

[R75] 导出环境变量
来源：http://hz.yj20258888.top/gtktwxrmqi.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.nanxuanxn.top/gtsalonqar.html

[R76] 使用临时文件
来源：http://hz.zdqjudy.top/gtdjnccsgz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zdqjudy.top/gtkalzeult.html

[R77] 读取用户输入
来源：http://hz.sweek.top/gtgrypwhbk.html

read -rp "请输入: " ans
来源：http://hz.birdmap.top/gtaoyckufy.html

[R78] 交互式菜单
来源：http://hz.xingfuxueyuan.xyz/gtulluqinp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xinyue.icu/gtyklxeugd.html

[R79] 解析命令行选项
来源：http://hz.guannengcc.top/gtefgrvina.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.andypj.xyz/gtmvrrlwhr.html

[R80] 查看脚本执行耗时
来源：http://hz.smart0.xyz/gtonclhliz.html

time ./run.sh
来源：http://hz.cucudq.cn/gtetqgxdin.html

================================================================================
来源：http://hz.xylfe.cn/gtigzywrzv.html

S. C / C++ 专题
来源：http://hz.tian-w.cn/gtbogluffq.html

================================================================================
来源：http://hz.mhx1999.top/gthjnrifir.html

[S01] C：Hello World
来源：http://hz.nanxinkj.top/gtwflvqxhr.html

#include <stdio.h>
来源：http://hz.ydjk.org.cn/gtffhefhxm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhoulong.xyz/gtnbhrydcc.html

[S02] C：变量与格式化输出
来源：http://hz.jinqigfzy.top/gtsbwtmtgv.html

int a = 10; printf("%d\n", a);
来源：http://hz.nanxinkj.top/gtljabfcbl.html

[S03] C：读入整数
来源：http://hz.nanxinkj.top/gthlepujxs.html

int x; scanf("%d", &x);
来源：http://hz.daxiang520.top/gtzoekopbn.html

[S04] C：字符串复制
来源：http://hz.ppjwa.cn/gteggohchv.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.quarkkingdee.top/gtmtkbvcwl.html

[S05] C：字符串长度
来源：http://hz.jiagoushi.top/gthljwjdrb.html

strlen(s)
来源：http://hz.jinyuanbaomall.cn/gtlyelqwmd.html

[S06] C：字符串比较
来源：http://hz.feifeiyinyue.top/gtdcbljrqw.html

strcmp(a, b) == 0
来源：http://hz.hnqzz.top/gttlieydru.html

[S07] C：数组遍历求和
来源：http://hz.ybcxt.top/gtbihardof.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jinghuilouyu.cn/gtjqmscgsj.html

[S08] C：动态内存分配与释放
来源：http://hz.shanyushiyangkeji.top/gtgnsqhfvq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.chenjidiqi.icu/gtcflcbkua.html

[S09] C：结构体定义与初始化
来源：http://hz.jqgufenzy.top/gtmgojixep.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.fengsongda.top/gtqlcmivvj.html

[S10] C：指针与解引用
来源：http://hz.andypj.xyz/gtfldwidwj.html

int *p = &a;  *p = 5;
来源：http://hz.haohaochexian.top/gtvrdnygxz.html

[S11] C：逐行读文件
来源：http://hz.xziqi.cn/gtiptcxtry.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jinqigufen.top/gttodsmjxl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.dashuyun.cn/gtbychanqu.html

fclose(f);
来源：http://hz.jlsjyb.cn/gtjwgsrzex.html

[S12] C：写文件
来源：http://hz.xuetiantiany.cn/gtygfuqrku.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jinyuanbaomall.cn/gtcwcjeduj.html

[S13] C：宏定义
来源：http://hz.snrcjt.cn/gtlpumqzwa.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.tanke756.top/gtsjzvnlnq.html

[S14] C：枚举
来源：http://hz.nanxinkj.top/gthsslgnwr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.sufxvd.cn/gtrssheqgq.html

[S15] C：类型转换
来源：http://hz.yuanzhike.top/gtivlfjpzt.html

(double) a / b
来源：http://hz.ywan-chungtsiang.top/gttmndcseb.html

[S16] C：位操作置位
来源：http://hz.sweek.top/gtftuapgqn.html

x |= (1 << 3);
来源：http://hz.guannengcc.top/gtgmuzfnlk.html

[S17] C：安全拼接字符串
来源：http://hz.xuetiantiany.cn/gtvkjxfleu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.chenzaomai.com/gteczivtus.html

[S18] C：命令行参数
来源：http://hz.ivvv.top/gtzxscexag.html

int main(int argc, char **argv)
来源：http://hz.xingfuxueyuan.xyz/gtljpcnbev.html

[S19] C：快速排序
来源：http://hz.yj20258.top/gtycttdjqg.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.tian-w.cn/gtzvmshwge.html

[S20] C：二分查找
来源：http://hz.sxryk.cn/gtylrmeyuy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jinqigufen.top/gtjgyrstyf.html

[S21] C：字符类别判断
来源：http://hz.snrcjt.cn/gtcsmflhqw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yongpay.top/gtvnwkrpew.html

[S22] C：字符串转数字
来源：http://hz.daxiang520.top/gtbtccospv.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.vqdsnc.cn/gtjjejoste.html

[S23] C：随机数
来源：http://hz.hfpthk.cn/gtxvnjhrvx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ydzc1.top/gtlbxipxix.html

[S24] C：获取本地时间
来源：http://hz.xingfuxueyuan.xyz/gtljbnidet.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.meibo888.top/gttizcktem.html

[S25] C：内存拷贝
来源：http://hz.guannengcc.top/gthrcdwfxg.html

memcpy(dst, src, n);
来源：http://hz.shzxlz.cn/gtgcilaswb.html

[S26] C：内存清零
来源：http://hz.andypj.xyz/gtfavesumr.html

memset(a, 0, sizeof a);
来源：http://hz.fengsongda.top/gtlapwngaa.html

[S27] C：定义常量
来源：http://hz.guowangkeji.top/gtdylmkcmk.html

const double PI = 3.14159;
来源：http://hz.ybcxt.top/gtfbbprhvy.html

[S28] C：静态变量
来源：http://hz.hongshengwenyu.top/gtggomvtpj.html

static int counter = 0;
来源：http://hz.yvedp.cn/gtfymkaqqs.html

[S29] C：变参函数
来源：http://hz.shzxlz.cn/gtvrdzgvcv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ydjk.org.cn/gtuujlgnzw.html

[S30] C：头文件保护
来源：http://hz.jinyuanbaomall.cn/gtivslgmdm.html

#ifndef X_H
来源：http://hz.guowangkeji.top/gtgdrirzhj.html

#define X_H
来源：http://hz.vqdsnc.cn/gtfcxafmwp.html

#endif
来源：http://hz.jqgufenzy.top/gtpeuwlqeb.html

[S31] C++：Hello World
来源：http://hz.tian-w.cn/gtsbqrwjof.html

#include <iostream>
来源：http://hz.sufxvd.cn/gtrdabdvot.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.gaohongyu789.top/gtwtmmwirk.html

[S32] C++：字符串
来源：http://hz.chenlongwang.top/gtmpujtsjn.html

std::string s = "hi";  s += "!";
来源：http://hz.jinyuanbaomall.cn/gthyfebosp.html

[S33] C++：vector 增删
来源：http://hz.quarkkingdee.top/gtqyzkruxg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.meibo888.top/gtefltwqro.html

[S34] C++：遍历 vector
来源：http://hz.jianghu66.top/gtcfzbknpv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jinghuilouyu.cn/gtxaeaxang.html

[S35] C++：map
来源：http://hz.gaohongyu789.top/gtxjbwyira.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hongshengwenyu.top/gtilyirbro.html

[S36] C++：unordered_map
来源：http://hz.zhijiandao.cn/gtlutlqijl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinghuilouyu.cn/gtypomzmwj.html

[S37] C++：set
来源：http://hz.sysykeji.top/gtxoqjdirr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhijiandao.cn/gtgksppwgk.html

[S38] C++：排序
来源：http://hz.jinqigufen.top/gtvlbieyog.html

std::sort(v.begin(), v.end());
来源：http://hz.jlsjyb.cn/gtpkmpgkqe.html

[S39] C++：自定义比较器排序
来源：http://hz.pengpengdd.cyou/gtbvloyxad.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yangfankeji.com/gtdfmurult.html

[S40] C++：查找元素
来源：http://hz.chenjidiqi.icu/gtshtkkvbx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.tian-w.cn/gtlawqtizv.html

[S41] C++：类与构造函数
来源：http://hz.cdnleiting.top/gtomaiqfub.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.52xcode.cn/gtjpaeqjhp.html

[S42] C++：继承与虚函数
来源：http://hz.yonumen.top/gtdjxuaaco.html

class B : public Base { public: void f() override {} };
来源：http://hz.wangdashe.top/gtdcdyzdvf.html

[S43] C++：智能指针
来源：http://hz.xinyue.icu/gtweldtzjk.html

auto p = std::make_unique<int>(5);
来源：http://hz.ehwqpu.com/gtkazisboo.html

[S44] C++：引用传参
来源：http://hz.ywan-chungtsiang.top/gtzexvrgbd.html

void inc(int &x) { ++x; }
来源：http://hz.ydzc1.top/gtovqptyuy.html

[S45] C++：lambda
来源：http://hz.cucudq.cn/gtudletkvy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.c1oappe.top/gtpkqlprfr.html

[S46] C++：函数模板
来源：http://hz.wangdashe.top/gtrzcfmfqc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hongshengwenyu.top/gtrrdgdfvr.html

[S47] C++：结构化绑定遍历
来源：http://hz.yuanzhike.top/gtwcnmfqyq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.pycfn.com/gtvlaqerzu.html

[S48] C++：逐行读文件
来源：http://hz.cqqwz.cn/gtrnojdowj.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenlongwang.top/gtzjrogomi.html

while (std::getline(in, line)) { }
来源：http://hz.ydzc1.top/gtxfugzlia.html

[S49] C++：写文件
来源：http://hz.zdqjudy.top/gtrqhtyybp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cucudq.cn/gtkbcxtsmk.html

[S50] C++：格式化数字
来源：http://hz.jyoumei.cn/gtqufnvclw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhaomingkeji.xyz/gtfsltdgim.html

[S51] C++：显式类型转换
来源：http://hz.chenjidiqi.icu/gtkmhzsfzs.html

static_cast<double>(a) / b
来源：http://hz.havefunace.top/gtmqhbtgij.html

[S52] C++：const 与 noexcept
来源：http://hz.yj20258888.top/gtfxmotktl.html

int size() const noexcept { return n_; }
来源：http://hz.zhaomingkeji.xyz/gtqlqbwyik.html

[S53] C++：移动语义
来源：http://hz.xuanzx.com/gttmdlqzvm.html

std::vector<int> w = std::move(v);
来源：http://hz.jqgufenzy.top/gtcrwcowds.html

[S54] C++：异常处理
来源：http://hz.pengpengdd.cyou/gtvicjtwxh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hywenlv.cn/gtpzsmvlye.html

[S55] C++：结构化绑定
来源：http://hz.0kj1m.cn/gtiipjcqev.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jyoumei.cn/gtuqxsmizn.html

[S56] C++：optional
来源：http://hz.nwbrower.top/gtrmcwmsde.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.smart0.xyz/gtgbtnmyur.html

[S57] C++：编译期常量
来源：http://hz.tian-w.cn/gteyggzrna.html

constexpr int N = 10;
来源：http://hz.zhixingplan.top/gtgbysewzi.html

[S58] C++：命名空间
来源：http://hz.chenjidiqi.icu/gtkevmlukq.html

namespace ns { int f() { return 1; } }
来源：http://hz.quarkkingdee.top/gtbfmbwgli.html

[S59] C++：静态断言
来源：http://hz.zhixingplan.top/gtwqdoswju.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yj202588.top/gtrgatihqc.html

[S60] C++：遍历并删除元素
来源：http://hz.hongshengwenyu.top/gtjdlpjjye.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.haohaochexian.top/gtttlnaeag.html

================================================================================
来源：http://hz.chenzaomai.com/gtnfmbxcda.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shanyushiyangtech.top/gtzniajhht.html

================================================================================
来源：http://hz.chenlongwang.top/gtkcrhsruy.html

[T01] Kotlin：Hello World
来源：http://hz.yj20258.top/gtxlxlgafc.html

println("Hello")
来源：http://hz.daria6918.cn/gtwvvsrtgj.html

[T02] Kotlin：变量
来源：http://hz.zhoulong.xyz/gtwypjpdpl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.wangdashe.top/gtdocdixpc.html

[T03] Kotlin：字符串模板
来源：http://hz.ivvv.top/gtrzmceivh.html

"值: $b"
来源：http://hz.jyoumei.cn/gtararrxgy.html

[T04] Kotlin：空安全
来源：http://hz.chenzaomai.com/gtzsfdmcpi.html

val n: String? = null;  n?.length
来源：http://hz.mhx1999.top/gtcamjbmus.html

[T05] Kotlin：when 表达式
来源：http://hz.haohaochexian.top/gtijdozgym.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhixingplan.top/gtxetgpcfs.html

[T06] Kotlin：集合映射
来源：http://hz.smart0.xyz/gtemgoevbi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.fengsongda.top/gtcpdmdmtf.html

[T07] Kotlin：集合过滤
来源：http://hz.shuidangran.top/gtpliedxen.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhijiandao.cn/gthqihbbmi.html

[T08] Kotlin：数据类
来源：http://hz.yj202588.top/gtdjgjhkuz.html

data class User(val name: String, val age: Int)
来源：http://hz.kuanghao11.cn/gtoqgylcuv.html

[T09] Kotlin：扩展函数
来源：http://hz.aibaodan.cn/gtltmibjra.html

fun String.exclaim() = this + "!"
来源：http://hz.ybcxt.top/gtrwczoiyc.html

[T10] Kotlin：默认参数
来源：http://hz.nanxuanxn.top/gtzhdcolzw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.fzhhl.top/gtbiropwub.html


<!-- 参考信息 -->