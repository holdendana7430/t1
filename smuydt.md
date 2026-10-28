代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://hz.daria6918.cn/gtlgwuzzym.html

[R14] C 风格 for
来源：http://hz.shuidangran.top/gtpadewibr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jqgufenzy.top/gtmcrifpvf.html

[R15] while 逐行读文件
来源：http://hz.kuanghao11.cn/gtddvsnbni.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.gzhubu.top/gttskvsqbf.html

[R16] until 等待条件
来源：http://hz.redwolf501.top/gtqthlsfls.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.kuanghao11.cn/gtjypdrzok.html

[R17] 数组定义与取值
来源：http://hz.jinqigufen.top/gtvvkhfgkj.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.svipenyu.cn/gtiyrzjxdy.html

[R18] 遍历数组
来源：http://hz.yonumen.top/gtahxbcixo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.chenlongwang.top/gtqlqgvqrv.html

[R19] 数组长度
来源：http://hz.hammf.cn/gthotsfxiz.html

echo "${#arr[@]}"
来源：http://hz.meibo888.top/gtwdjdsdja.html

[R20] 关联数组（字典）
来源：http://hz.mhx1999.top/gtsyxpkulq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.316326.xyz/gtgwiyrxju.html

[R21] 字符串长度
来源：http://hz.pengpengdd.cyou/gtrjdzztgn.html

echo "${#s}"
来源：http://hz.0kj1m.cn/gtkbsgexhs.html

[R22] 截取子串
来源：http://hz.zhaomingkeji.xyz/gtqzljjgdp.html

echo "${s:0:5}"
来源：http://hz.jinqigufen.top/gtcurpffjx.html

[R23] 字符串替换
来源：http://hz.xingfuxueyuan.xyz/gthgixwfyu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.aibaodan.cn/gtozbxiziu.html

[R24] 大小写转换
来源：http://hz.nanxinkj.top/gtobouwelf.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.nwbrower.top/gtxzsuunqw.html

[R25] 去后缀 / 去前缀
来源：http://hz.shanyushiyangtech.top/gtotlmxoov.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jianghu66.top/gtegjkhpfi.html

[R26] 命令替换
来源：http://hz.birdmap.top/gttpnpfyll.html

now=$(date +%F); echo "$now"
来源：http://hz.0kj1m.cn/gtoztdauhb.html

[R27] 算术展开
来源：http://hz.gaohongyu789.top/gtbyowuzqz.html

echo $((1 + 2 * 3))
来源：http://hz.daxiang520.top/gtcgcrxbqf.html

[R28] 浮点运算
来源：http://hz.yuanzhike.top/gtfoykrbmi.html

echo "scale=2; 10/3" | bc
来源：http://hz.gogol.net.cn/gtxkgfzzdf.html

[R29] 定义函数
来源：http://hz.aizwys.cn/gtowinsfnm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jqgfzy.top/gtfhjodahk.html

[R30] 函数返回状态码
来源：http://hz.zhongyouzk.top/gttnamqiod.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gogol.net.cn/gtuqsxnzzw.html

[R31] 局部变量
来源：http://hz.sxryk.cn/gtwagormjt.html

f() { local x=1; echo "$x"; }
来源：http://hz.hnxiangtu.top/gtdtvzgsoy.html

[R32] 参数个数校验
来源：http://hz.daria6918.cn/gtirmrmjrj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.gogol.net.cn/gtsxjhmwyl.html

[R33] 捕获错误并提示行号
来源：http://hz.jinqigufen.top/gteozxofew.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gogol.net.cn/gtshbkpkwn.html

[R34] 退出时清理
来源：http://hz.iojbl.cn/gtkvuiodak.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhixingplan.top/gtxfacsimu.html

[R35] 后台执行并等待
来源：http://hz.zdqjudy.top/gtqirvtlzj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shanyushiyangtech.top/gtjevatkdt.html

[R36] 并发执行多个任务
来源：http://hz.52xcode.cn/gtmonlfirz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hammf.cn/gtvnheniab.html

[R37] 把输出赋给变量
来源：http://hz.iojbl.cn/gtondxuwqk.html

files=$(ls -1)
来源：http://hz.ywan-chungtsiang.top/gtiydnhzou.html

[R38] 管道串联
来源：http://hz.dianchejie.cn/gtohgfemft.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sufxvd.cn/gtfjoghlhz.html

[R39] 重定向标准输出与错误
来源：http://hz.gzhubu.top/gtekdhydej.html

cmd > out.log 2>&1
来源：http://hz.jianghu66.top/gteeuxtenh.html

[R40] 追加写日志
来源：http://hz.ybcxt.top/gtyvzdmdnh.html

echo "log" >> out.log
来源：http://hz.gaohongyu789.top/gtogxdcfzz.html

[R41] 丢弃输出
来源：http://hz.gaohongyu789.top/gtxfpewlqn.html

cmd >/dev/null 2>&1
来源：http://hz.ydzc1.top/gtoerrwgft.html

[R42] 输入重定向
来源：http://hz.jqgfzy.top/gtomqkecas.html

wc -l < a.txt
来源：http://hz.tanke756.top/gtdhudegdj.html

[R43] 按名字查找文件
来源：http://hz.sweek.top/gtpiblwcht.html

find . -name "*.log" -type f
来源：http://hz.pengpengdd.cyou/gticcfgxks.html

[R44] 按修改时间查找
来源：http://hz.9152youxi.cn/gtcoynwyrc.html

find . -mtime -7 -type f
来源：http://hz.quarkkingdee.top/gtjewvgoua.html

[R45] 批量删除
来源：http://hz.jiagoushi.top/gtfqohzgdq.html

find . -name "*.tmp" -delete
来源：http://hz.316326.xyz/gtekekfizd.html

[R46] 递归替换文件内容
来源：http://hz.dashuyun.cn/gttrsyooyr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hongshengwenyu.top/gtdvyzgnmk.html

[R47] sed 单行替换
来源：http://hz.xziqi.cn/gtabogjhyp.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yonumen.top/gtumelenfs.html

[R48] awk 取指定列
来源：http://hz.hammf.cn/gtkeroyknh.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhoulong.xyz/gtpgyoulyr.html

[R49] awk 带条件
来源：http://hz.xuanzx.com/gthonedlfd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cheryme.top/gtapuesqtw.html

[R50] awk 求和
来源：http://hz.haohaochexian.top/gtpnlawlez.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ivvv.top/gtafjocjof.html

[R51] 排序去重取前几
来源：http://hz.aibaodan.cn/gtqqkoajow.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yj20258.top/gtwebtjbcv.html

[R52] 统计行数
来源：http://hz.cheryme.top/gthmeietze.html

wc -l a.txt
来源：http://hz.gaohongyu789.top/gtzmydnzci.html

[R53] 查看文件头与实时尾
来源：http://hz.mhx1999.top/gtiupwiggz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.c1oappe.top/gtqasbopuc.html

[R54] 比较两个文件
来源：http://hz.yonumen.top/gtyvgumjpq.html

diff a.txt b.txt
来源：http://hz.guowangkeji.top/gtkqnkvljv.html

[R55] 压缩与解压
来源：http://hz.nwbrower.top/gtfhwaddcd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhiwuduotai.top/gtmhytyvrd.html

[R56] 远程拷贝
来源：http://hz.sufxvd.cn/gtwdhaggjj.html

scp file user@host:/path/
来源：http://hz.zhongyouzk.top/gtbmmtlhzv.html

[R57] 远程执行命令
来源：http://hz.iojbl.cn/gtbvhruics.html

ssh user@host 'uptime'
来源：http://hz.zhongyouzk.top/gtnxnuywnc.html

[R58] 下载文件
来源：http://hz.jinqigfzy.top/gtzllrtvda.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.pycfn.com/gtladxxpqy.html

[R59] 发 POST JSON
来源：http://hz.chenlongwang.top/gttuyzoudp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.daria6918.cn/gtjnweljir.html

[R60] 只看 HTTP 状态码
来源：http://hz.aizwys.cn/gtkwmyskdw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shuidangran.top/gtbyvmmxjq.html

[R61] 磁盘占用
来源：http://hz.redwolf501.top/gtlqbgtpsc.html

df -h;  du -sh *
来源：http://hz.feifeiyinyue.top/gtgfkhiaac.html

[R62] 找最占空间的文件
来源：http://hz.sxryk.cn/gthohrolmh.html

du -ah . | sort -rh | head -10
来源：http://hz.chenlongwang.top/gtililrzhu.html

[R63] 内存与进程
来源：http://hz.jiagoushi.top/gtknuongzr.html

free -h;  ps aux | grep nginx
来源：http://hz.tian-w.cn/gtwdzhofza.html

[R64] 结束进程
来源：http://hz.shzxlz.cn/gtkhjxncsi.html

kill -9 $(pgrep -f app.py)
来源：http://hz.wangdashe.top/gtmptprbrn.html

[R65] 查看端口占用
来源：http://hz.svipenyu.cn/gtchkeaycq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ydzc1.top/gtqhjwnthu.html

[R66] 定时任务
来源：http://hz.gaohongyu789.top/gtcaenpvjt.html

crontab -e;  crontab -l
来源：http://hz.gzhubu.top/gtdymexgxg.html

[R67] 生成随机十六进制串
来源：http://hz.yj20258888.top/gtrzyjrnmt.html

openssl rand -hex 16
来源：http://hz.guowangkeji.top/gtedtdcywm.html

[R68] 计算文件校验值
来源：http://hz.quarkkingdee.top/gthwyeyzeb.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhiwuduotai.top/gtsmsyhsyb.html

[R69] 生成随机密码
来源：http://hz.hysaishi.cn/gtyxjpfwpv.html

head -c 16 /dev/urandom | base64
来源：http://hz.cucudq.cn/gtvjroefqu.html

[R70] 时间戳与互转
来源：http://hz.snrcjt.cn/gtzaraymmn.html

date +%s;  date -d @1700000000
来源：http://hz.ybcxt.top/gtpvexbizq.html

[R71] 日期格式化
来源：http://hz.andypj.xyz/gtxteclzge.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gotoacloud.top/gtufdbyfnm.html

[R72] 等待端口就绪
来源：http://hz.sweek.top/gtiypdpgyp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hywenlv.cn/gttkrlmyzc.html

[R73] 分割大日志
来源：http://hz.xingfuxueyuan.xyz/gtekuzjezx.html

split -l 1000 big.log part_
来源：http://hz.jqgufenzy.top/gtshrkdwrm.html

[R74] 批量重命名
来源：http://hz.jiagoushi.top/gtuydyohbj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zdqjudy.top/gtwcrxywps.html

[R75] 导出环境变量
来源：http://hz.316326.xyz/gtgpfwdjip.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yueranfly.top/gtpirswsgo.html

[R76] 使用临时文件
来源：http://hz.cdnleiting.top/gtiiccsknj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yuxming.cn/gtartknukc.html

[R77] 读取用户输入
来源：http://hz.feifeiyinyue.top/gtzwsqgqjr.html

read -rp "请输入: " ans
来源：http://hz.havefunace.top/gtaijbuucu.html

[R78] 交互式菜单
来源：http://hz.andypj.xyz/gtvecnavkr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shanyushiyangkeji.top/gtakykchkm.html

[R79] 解析命令行选项
来源：http://hz.jianghu66.top/gtymftjokc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.haohaochexian.top/gteiiwirap.html

[R80] 查看脚本执行耗时
来源：http://hz.sysykeji.top/gtyubhydcn.html

time ./run.sh
来源：http://hz.hammf.cn/gtjjlwndtu.html

================================================================================
来源：http://hz.smart0.xyz/gtkmefrxoa.html

S. C / C++ 专题
来源：http://hz.cdnleiting.top/gtmnwoumkg.html

================================================================================
来源：http://hz.yuanzhike.top/gtsgfbuidd.html

[S01] C：Hello World
来源：http://hz.xuetiantiany.cn/gtzkpjpqye.html

#include <stdio.h>
来源：http://hz.hysaishi.cn/gthrsjexsh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jinyuanbaomall.cn/gtoqzlffbc.html

[S02] C：变量与格式化输出
来源：http://hz.hnxiangtu.top/gtjrsxiyas.html

int a = 10; printf("%d\n", a);
来源：http://hz.nanxuanxn.top/gtyfsxxkpd.html

[S03] C：读入整数
来源：http://hz.ydjk.org.cn/gtwzhtmxgw.html

int x; scanf("%d", &x);
来源：http://hz.daria6918.cn/gtpyetglsw.html

[S04] C：字符串复制
来源：http://hz.9152youxi.cn/gtxrytgpst.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.52xcode.cn/gtqvoyeazh.html

[S05] C：字符串长度
来源：http://hz.ydjk.org.cn/gtszssrgft.html

strlen(s)
来源：http://hz.pycfn.com/gtydmfieru.html

[S06] C：字符串比较
来源：http://hz.hywenlv.cn/gtysiqihpf.html

strcmp(a, b) == 0
来源：http://hz.hnxiangtu.top/gthkrpfjpt.html

[S07] C：数组遍历求和
来源：http://hz.yuxming.cn/gtkrxosuzt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhixingplan.top/gtolwnnuhc.html

[S08] C：动态内存分配与释放
来源：http://hz.shanyushiyangtech.top/gttfawfnty.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xingfuxueyuan.xyz/gtbbgiiyxk.html

[S09] C：结构体定义与初始化
来源：http://hz.andypj.xyz/gtgipncaeu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cqqwz.cn/gtpnrwlqsz.html

[S10] C：指针与解引用
来源：http://hz.ehwqpu.com/gtfefjmhfs.html

int *p = &a;  *p = 5;
来源：http://hz.gaohongyu789.top/gtelidxnzp.html

[S11] C：逐行读文件
来源：http://hz.shangyingyoupin.top/gtwhbhepmg.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhongyouzk.top/gtmgngolkv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ybcxt.top/gtkwzjrwrx.html

fclose(f);
来源：http://hz.shangyingyoupin.top/gtoogixgeo.html

[S12] C：写文件
来源：http://hz.yj20258.top/gtndouftvp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.c1oappe.top/gtxpxbqgrl.html

[S13] C：宏定义
来源：http://hz.sxryk.cn/gtjnoolxdm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hywenlv.cn/gtqsurgxoq.html

[S14] C：枚举
来源：http://hz.iojbl.cn/gtjzjlqcvs.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ppjwa.cn/gtczdcxkin.html

[S15] C：类型转换
来源：http://hz.sxryk.cn/gtesdhngvw.html

(double) a / b
来源：http://hz.ywan-chungtsiang.top/gteskuecfe.html

[S16] C：位操作置位
来源：http://hz.birdmap.top/gtpoeaclzl.html

x |= (1 << 3);
来源：http://hz.yueranfly.top/gtbbxprxbf.html

[S17] C：安全拼接字符串
来源：http://hz.shanyushiyangtech.top/gtebaijeuc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hongshengwenyu.top/gtfltbdhas.html

[S18] C：命令行参数
来源：http://hz.shanyushiyangkeji.top/gtpctoxoit.html

int main(int argc, char **argv)
来源：http://hz.sysykeji.top/gtttguyqjj.html

[S19] C：快速排序
来源：http://hz.hnxiangtu.top/gtsssxvotp.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.snrcjt.cn/gtfkcycbkf.html

[S20] C：二分查找
来源：http://hz.jyoumei.cn/gtdcgldpkp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.fzhhl.top/gtjyjfpbpm.html

[S21] C：字符类别判断
来源：http://hz.nwbrower.top/gtuvzipunp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.cheryme.top/gthsubsgze.html

[S22] C：字符串转数字
来源：http://hz.yuanzhike.top/gtqzcgnavu.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ydzc1.top/gtpczdwqyz.html

[S23] C：随机数
来源：http://hz.hongshengwenyu.top/gtfppjhldb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.sxryk.cn/gtqyeikols.html

[S24] C：获取本地时间
来源：http://hz.jinqigufen.top/gtqmqrnnwt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yongpay.top/gtzmxgrmev.html

[S25] C：内存拷贝
来源：http://hz.shuidangran.top/gtxdrogbhu.html

memcpy(dst, src, n);
来源：http://hz.gogol.net.cn/gtbgzxhozy.html

[S26] C：内存清零
来源：http://hz.yangfankeji.com/gtwogaqkja.html

memset(a, 0, sizeof a);
来源：http://hz.xinyue.icu/gtgbukvkzr.html

[S27] C：定义常量
来源：http://hz.wangshuangyany.cn/gtparaiizi.html

const double PI = 3.14159;
来源：http://hz.yuxming.cn/gtzqstnlir.html

[S28] C：静态变量
来源：http://hz.jinqigfzy.top/gtxsvvhlrw.html

static int counter = 0;
来源：http://hz.cdnleiting.top/gtzlkbnzxw.html

[S29] C：变参函数
来源：http://hz.bjfxy.top/gtgimjtohr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhixingplan.top/gtxxgmyrfg.html

[S30] C：头文件保护
来源：http://hz.yvedp.cn/gtyiwvvwly.html

#ifndef X_H
来源：http://hz.wangdashe.top/gtseeulenc.html

#define X_H
来源：http://hz.nanxinkj.top/gtcwluziry.html

#endif
来源：http://hz.sxryk.cn/gtzwaeivju.html

[S31] C++：Hello World
来源：http://hz.kuanghao11.cn/gttkogmdlp.html

#include <iostream>
来源：http://hz.guannengcc.top/gtipohnxaw.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zdqjudy.top/gtwsunrfad.html

[S32] C++：字符串
来源：http://hz.guowangkeji.top/gtbbnyuvav.html

std::string s = "hi";  s += "!";
来源：http://hz.meibo888.top/gtqwofymbp.html

[S33] C++：vector 增删
来源：http://hz.sufxvd.cn/gtmnkfwizl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.redwolf501.top/gtiorplfvb.html

[S34] C++：遍历 vector
来源：http://hz.wangshuangyany.cn/gtjoznnxie.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yueranfly.top/gtnrsinhcu.html

[S35] C++：map
来源：http://hz.snrcjt.cn/gtgslbbyhu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hnqzz.top/gtgtmxktcv.html

[S36] C++：unordered_map
来源：http://hz.smart0.xyz/gtaxqjneqq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gogol.net.cn/gtqrtblqct.html

[S37] C++：set
来源：http://hz.smart0.xyz/gtvfgntsrg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cheryme.top/gtupycekxp.html

[S38] C++：排序
来源：http://hz.ywan-chungtsiang.top/gtijrslmsg.html

std::sort(v.begin(), v.end());
来源：http://hz.hammf.cn/gtueyfeiqj.html

[S39] C++：自定义比较器排序
来源：http://hz.nwbrower.top/gtmnjaymfg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.smart0.xyz/gtvbrtnihf.html

[S40] C++：查找元素
来源：http://hz.jinghuilouyu.cn/gtulisesac.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cqqwz.cn/gtbxwbaswo.html

[S41] C++：类与构造函数
来源：http://hz.yongpay.top/gtvitevnvm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.dianchejie.cn/gtgrjiktes.html

[S42] C++：继承与虚函数
来源：http://hz.xinyue.icu/gtvlwuefon.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhoulong.xyz/gtsatcibkh.html

[S43] C++：智能指针
来源：http://hz.bjfxy.top/gtoylfcmsz.html

auto p = std::make_unique<int>(5);
来源：http://hz.vqdsnc.cn/gtafzdvkcm.html

[S44] C++：引用传参
来源：http://hz.yj20258.top/gtcorvbbhx.html

void inc(int &x) { ++x; }
来源：http://hz.svipenyu.cn/gtaduvkuqq.html

[S45] C++：lambda
来源：http://hz.tian-w.cn/gtatmeibyi.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xuanzx.com/gtrivgdzkh.html

[S46] C++：函数模板
来源：http://hz.ehwqpu.com/gtomwdznzx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhoulong.xyz/gtpynqtbjx.html

[S47] C++：结构化绑定遍历
来源：http://hz.hongshengwenyu.top/gtfftcxitt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.pycfn.com/gtbsjhqyla.html

[S48] C++：逐行读文件
来源：http://hz.haohaochexian.top/gtlkxlpfih.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shanyushiyangtech.top/gtjsschafz.html

while (std::getline(in, line)) { }
来源：http://hz.nanxinkj.top/gtibsyjwip.html

[S49] C++：写文件
来源：http://hz.shanyushiyangkeji.top/gtzqirsvqn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhaomingkeji.xyz/gtskbcymbj.html

[S50] C++：格式化数字
来源：http://hz.316326.xyz/gtpqdbbtuj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.vqdsnc.cn/gthhyinftm.html

[S51] C++：显式类型转换
来源：http://hz.shanyushiyangkeji.top/gtpgetrpju.html

static_cast<double>(a) / b
来源：http://hz.shuidangran.top/gtjfmiybsn.html

[S52] C++：const 与 noexcept
来源：http://hz.ydjk.org.cn/gtemhotjkc.html

int size() const noexcept { return n_; }
来源：http://hz.hammf.cn/gtgxzzwkof.html

[S53] C++：移动语义
来源：http://hz.cdnleiting.top/gtsqyfrrow.html

std::vector<int> w = std::move(v);
来源：http://hz.smart0.xyz/gtjsvonruz.html

[S54] C++：异常处理
来源：http://hz.jiagoushi.top/gtppghntrq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.wangdashe.top/gtsmebbxvl.html

[S55] C++：结构化绑定
来源：http://hz.ydzc1.top/gtikyudjxo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.sysykeji.top/gthoxrvqic.html

[S56] C++：optional
来源：http://hz.yvedp.cn/gtfcgclvgd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhiwuduotai.top/gtomzjspxs.html

[S57] C++：编译期常量
来源：http://hz.gzhubu.top/gtmitskwqr.html

constexpr int N = 10;
来源：http://hz.hywenlv.cn/gturzwxaas.html

[S58] C++：命名空间
来源：http://hz.cdnleiting.top/gtjvdikozb.html

namespace ns { int f() { return 1; } }
来源：http://hz.daxiang520.top/gthvluajnw.html

[S59] C++：静态断言
来源：http://hz.zhijiandao.cn/gtayptzemy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ybcxt.top/gttlyrvsyq.html

[S60] C++：遍历并删除元素
来源：http://hz.aibaodan.cn/gtwddnccoa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ehwqpu.com/gtfvvsbdzi.html

================================================================================
来源：http://hz.ppjwa.cn/gtvafapead.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cucudq.cn/gthjfxiiik.html

================================================================================
来源：http://hz.zycfv.cn/gtwfkvmnhc.html

[T01] Kotlin：Hello World
来源：http://hz.wangshuangyany.cn/gthdmtpooz.html

println("Hello")
来源：http://hz.mhx1999.top/gttrhlynlc.html

[T02] Kotlin：变量
来源：http://hz.jlsjyb.cn/gtswvmdfwg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hongshengwenyu.top/gtncoceqtm.html

[T03] Kotlin：字符串模板
来源：http://hz.andypj.xyz/gtapfqrjus.html

"值: $b"
来源：http://hz.tian-w.cn/gtyvqmysrj.html

[T04] Kotlin：空安全
来源：http://hz.zdqjudy.top/gtxvxeeqsd.html

val n: String? = null;  n?.length
来源：http://hz.daria6918.cn/gtpfsvprno.html

[T05] Kotlin：when 表达式
来源：http://hz.ydzc1.top/gttyvtllpk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yj202588.top/gtaaktkpjr.html

[T06] Kotlin：集合映射
来源：http://hz.jqgfzy.top/gtpcskojhl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jiagoushi.top/gtvogxhqjc.html

[T07] Kotlin：集合过滤
来源：http://hz.pycfn.com/gtafippklp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.kuanghao11.cn/gtsmzldagd.html

[T08] Kotlin：数据类
来源：http://hz.tian-w.cn/gtkjuxcudu.html

data class User(val name: String, val age: Int)
来源：http://hz.ydjk.org.cn/gtprrdqzoh.html

[T09] Kotlin：扩展函数
来源：http://hz.sxryk.cn/gtfsoxsnvr.html

fun String.exclaim() = this + "!"
来源：http://hz.feifeiyinyue.top/gtvbsrchmq.html

[T10] Kotlin：默认参数
来源：http://hz.svipenyu.cn/gtyabdqkhh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yueranfly.top/gtuuodaako.html

[T11] Kotlin：协程
来源：http://hz.gogol.net.cn/gtctfqgvkt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.gaohongyu789.top/gtlrzfjclz.html

[T12] Kotlin：解构声明
来源：http://hz.haohaochexian.top/gtgzbzcupw.html

val (a, b) = Pair(1, 2)
来源：http://hz.chenlongwang.top/gtfutssrcx.html

[T13] Kotlin：只读 Map
来源：http://hz.shuidangran.top/gtgtqhbjrm.html

val m = mapOf("a" to 1)
来源：http://hz.chenjidiqi.icu/gtebyahpsu.html

[T14] Kotlin：循环
来源：http://hz.jinqigufen.top/gthpdifldo.html

for (i in 1..10) println(i)
来源：http://hz.pycfn.com/gtpipihgkx.html

[T15] Kotlin：接口
来源：http://hz.jinqigfzy.top/gtvoloqmhb.html

interface Shape { fun area(): Double }
来源：http://hz.svipenyu.cn/gtlcrewdag.html

[T16] Swift：Hello World
来源：http://hz.wangdashe.top/gttkwknwoe.html

print("Hello")
来源：http://hz.tianlin.xyz/gtosfcrwgi.html


<!-- 参考信息 -->