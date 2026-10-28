代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://hz.ydjk.org.cn/gtiblmrdlo.html

[R14] C 风格 for
来源：http://hz.cdnleiting.top/gtiksbmshy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yj20258888.top/gtqxzzjhrw.html

[R15] while 逐行读文件
来源：http://hz.redwolf501.top/gtykylxgid.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ydjk.org.cn/gttnvoqkoq.html

[R16] until 等待条件
来源：http://hz.shangyingyoupin.top/gtlrrumedz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.pycfn.com/gtdhruphwa.html

[R17] 数组定义与取值
来源：http://hz.yj20258.top/gtlwrphtgw.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jqgfzy.top/gtywxgbrmi.html

[R18] 遍历数组
来源：http://hz.jinqigufen.top/gtxvgtbscw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.smart0.xyz/gtjocgczvo.html

[R19] 数组长度
来源：http://hz.ydzc1.top/gtczkuxtkv.html

echo "${#arr[@]}"
来源：http://hz.quarkkingdee.top/gtoktnjjfn.html

[R20] 关联数组（字典）
来源：http://hz.pengpengdd.cyou/gtvaqxvcus.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shangyingyoupin.top/gtogqvgxfw.html

[R21] 字符串长度
来源：http://hz.gaohongyu789.top/gtffydhchy.html

echo "${#s}"
来源：http://hz.meibo888.top/gtspdkemlw.html

[R22] 截取子串
来源：http://hz.nanxinkj.top/gtnrrszwob.html

echo "${s:0:5}"
来源：http://hz.ydjk.org.cn/gtflwbtikr.html

[R23] 字符串替换
来源：http://hz.zhengqikj.top/gtzguoiyot.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sxryk.cn/gtyjvzoaef.html

[R24] 大小写转换
来源：http://hz.gzhubu.top/gtbsfhdjio.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.svipenyu.cn/gtbrkgbclo.html

[R25] 去后缀 / 去前缀
来源：http://hz.yangfankeji.com/gtetyuphuk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.mhx1999.top/gtocmsmkyh.html

[R26] 命令替换
来源：http://hz.ybcxt.top/gttczxhoht.html

now=$(date +%F); echo "$now"
来源：http://hz.gaohongyu789.top/gtmngovlbw.html

[R27] 算术展开
来源：http://hz.ppjwa.cn/gtvmudlddl.html

echo $((1 + 2 * 3))
来源：http://hz.jinyuanbaomall.cn/gttmdxulkm.html

[R28] 浮点运算
来源：http://hz.aizwys.cn/gtmnpnnnro.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhixingplan.top/gtnfsxjtro.html

[R29] 定义函数
来源：http://hz.guannengcc.top/gtxmjqqwji.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shangyingyoupin.top/gtbnxxyebb.html

[R30] 函数返回状态码
来源：http://hz.shangyingyoupin.top/gtneptyugq.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jinqigfzy.top/gtitktdncw.html

[R31] 局部变量
来源：http://hz.jiagoushi.top/gterhoqoty.html

f() { local x=1; echo "$x"; }
来源：http://hz.daria6918.cn/gtjskufzja.html

[R32] 参数个数校验
来源：http://hz.nanxinkj.top/gtmqgmiovv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.meibo888.top/gtyguxbhau.html

[R33] 捕获错误并提示行号
来源：http://hz.hysaishi.cn/gtxgkjihji.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.birdmap.top/gtoddzyyho.html

[R34] 退出时清理
来源：http://hz.cqqwz.cn/gteripjgsd.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zdqjudy.top/gtbxxmijir.html

[R35] 后台执行并等待
来源：http://hz.xziqi.cn/gtofthaugc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hongshengwenyu.top/gtpsniwdnp.html

[R36] 并发执行多个任务
来源：http://hz.daxiang520.top/gtjjltiaqt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jqgfzy.top/gteqvbkhls.html

[R37] 把输出赋给变量
来源：http://hz.meibo888.top/gtuazquyuo.html

files=$(ls -1)
来源：http://hz.gotoacloud.top/gtrsjcatvd.html

[R38] 管道串联
来源：http://hz.pycfn.com/gtzycvmmnc.html

cat a.txt | grep -i error | wc -l
来源：http://hz.9152youxi.cn/gtixzwxprz.html

[R39] 重定向标准输出与错误
来源：http://hz.gogol.net.cn/gtdvnaepeb.html

cmd > out.log 2>&1
来源：http://hz.yueranfly.top/gtsqzckaiu.html

[R40] 追加写日志
来源：http://hz.xinyue.icu/gtufjndrhc.html

echo "log" >> out.log
来源：http://hz.gotoacloud.top/gtxpfpuroe.html

[R41] 丢弃输出
来源：http://hz.daria6918.cn/gthvgdgqmk.html

cmd >/dev/null 2>&1
来源：http://hz.guannengcc.top/gtqolyvrai.html

[R42] 输入重定向
来源：http://hz.yongpay.top/gttrnvlufc.html

wc -l < a.txt
来源：http://hz.tanke756.top/gtqcujozrt.html

[R43] 按名字查找文件
来源：http://hz.tanke756.top/gtzannsijm.html

find . -name "*.log" -type f
来源：http://hz.kuanghao11.cn/gtqzuzvgjf.html

[R44] 按修改时间查找
来源：http://hz.hnqzz.top/gtktmmpmxi.html

find . -mtime -7 -type f
来源：http://hz.zhoulong.xyz/gtyohikfrl.html

[R45] 批量删除
来源：http://hz.gaohongyu789.top/gtcjdruakk.html

find . -name "*.tmp" -delete
来源：http://hz.jyoumei.cn/gtgoikufiy.html

[R46] 递归替换文件内容
来源：http://hz.ywan-chungtsiang.top/gtiadwneff.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.52xcode.cn/gtkdfswpbu.html

[R47] sed 单行替换
来源：http://hz.sweek.top/gtbgqsqoem.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.c1oappe.top/gtxtupxizh.html

[R48] awk 取指定列
来源：http://hz.yuxming.cn/gtqilyvjlp.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhixingplan.top/gtoyxobdrf.html

[R49] awk 带条件
来源：http://hz.shangyingyoupin.top/gtpocvkdaz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.tanke756.top/gtsptziysp.html

[R50] awk 求和
来源：http://hz.sxryk.cn/gtottaesag.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yj20258888.top/gtehvuayon.html

[R51] 排序去重取前几
来源：http://hz.xingfuxueyuan.xyz/gtffnbvkab.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.snrcjt.cn/gtspuinjkv.html

[R52] 统计行数
来源：http://hz.zhoulong.xyz/gtokhmhuyd.html

wc -l a.txt
来源：http://hz.52xcode.cn/gtldxzhjhx.html

[R53] 查看文件头与实时尾
来源：http://hz.sxryk.cn/gtqxdsfkfb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.gotoacloud.top/gtnmdepkgs.html

[R54] 比较两个文件
来源：http://hz.yuxming.cn/gtdkqrvynq.html

diff a.txt b.txt
来源：http://hz.yvedp.cn/gtufpsvjuf.html

[R55] 压缩与解压
来源：http://hz.jqgfzy.top/gtrlcvnxly.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yangfankeji.com/gtgprqrhfm.html

[R56] 远程拷贝
来源：http://hz.0kj1m.cn/gtactxarja.html

scp file user@host:/path/
来源：http://hz.ydzc1.top/gtqddyjirg.html

[R57] 远程执行命令
来源：http://hz.jiagoushi.top/gtulalknhh.html

ssh user@host 'uptime'
来源：http://hz.bjfxy.top/gtbasjggou.html

[R58] 下载文件
来源：http://hz.zhijiandao.cn/gtfjyrzznm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yvedp.cn/gttghpdyun.html

[R59] 发 POST JSON
来源：http://hz.cdnleiting.top/gthgjgezdj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hywenlv.cn/gtdgmmuysd.html

[R60] 只看 HTTP 状态码
来源：http://hz.vqdsnc.cn/gtnktwfoqi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.daria6918.cn/gtmikiuvrc.html

[R61] 磁盘占用
来源：http://hz.jianghu66.top/gtkhffjjes.html

df -h;  du -sh *
来源：http://hz.hysaishi.cn/gtxgdlygju.html

[R62] 找最占空间的文件
来源：http://hz.c1oappe.top/gthbkepdbx.html

du -ah . | sort -rh | head -10
来源：http://hz.52xcode.cn/gtdmyhitoo.html

[R63] 内存与进程
来源：http://hz.haohaochexian.top/gtezvwaykt.html

free -h;  ps aux | grep nginx
来源：http://hz.zdqjudy.top/gtppnqmsxl.html

[R64] 结束进程
来源：http://hz.jinqigufen.top/gtunjrbomf.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinqigfzy.top/gtvongjhdb.html

[R65] 查看端口占用
来源：http://hz.vqdsnc.cn/gtxqhtsywk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.guowangkeji.top/gtgnupwpzz.html

[R66] 定时任务
来源：http://hz.gogol.net.cn/gtihqdfvet.html

crontab -e;  crontab -l
来源：http://hz.yj20258.top/gtkgmxttsu.html

[R67] 生成随机十六进制串
来源：http://hz.ywan-chungtsiang.top/gtajifqgzc.html

openssl rand -hex 16
来源：http://hz.hnqzz.top/gtjivekrya.html

[R68] 计算文件校验值
来源：http://hz.hysaishi.cn/gtfnitpgcg.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.tianlin.xyz/gtmkquhrze.html

[R69] 生成随机密码
来源：http://hz.shangyingyoupin.top/gtlvpkpulq.html

head -c 16 /dev/urandom | base64
来源：http://hz.feifeiyinyue.top/gtsossqhvl.html

[R70] 时间戳与互转
来源：http://hz.hongshengwenyu.top/gttcmjfpjx.html

date +%s;  date -d @1700000000
来源：http://hz.guowangkeji.top/gtzkntwlwy.html

[R71] 日期格式化
来源：http://hz.snrcjt.cn/gtxzxtirgj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhiwuduotai.top/gtudnbyuin.html

[R72] 等待端口就绪
来源：http://hz.yanxiufei.cn/gtekrjjoty.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.shzxlz.cn/gtmurqytgb.html

[R73] 分割大日志
来源：http://hz.shangyingyoupin.top/gtsyepuera.html

split -l 1000 big.log part_
来源：http://hz.smart0.xyz/gtmzzkauvs.html

[R74] 批量重命名
来源：http://hz.kuanghao11.cn/gtnvpafohc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.svipenyu.cn/gtuldkiwaa.html

[R75] 导出环境变量
来源：http://hz.jinghuilouyu.cn/gtdiypvnkl.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.gaohongyu789.top/gtqvzyqiyw.html

[R76] 使用临时文件
来源：http://hz.meibo888.top/gtxsaoqpqg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jlsjyb.cn/gtlxznrdno.html

[R77] 读取用户输入
来源：http://hz.cashguo.top/gtsdxjbwti.html

read -rp "请输入: " ans
来源：http://hz.sysykeji.top/gtjxkebvap.html

[R78] 交互式菜单
来源：http://hz.smart0.xyz/gtrqbxdwbd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hysaishi.cn/gtwludllrm.html

[R79] 解析命令行选项
来源：http://hz.ydjk.org.cn/gtmzrxncld.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xinyue.icu/gtkzcebafp.html

[R80] 查看脚本执行耗时
来源：http://hz.9152youxi.cn/gtvafhvlbh.html

time ./run.sh
来源：http://hz.yuanzhike.top/gtbevssczc.html

================================================================================
来源：http://hz.wangdashe.top/gtlzcxqpex.html

S. C / C++ 专题
来源：http://hz.nanxinkj.top/gterdumnhp.html

================================================================================
来源：http://hz.cdnleiting.top/gtrnfxrpss.html

[S01] C：Hello World
来源：http://hz.0kj1m.cn/gtidrepytz.html

#include <stdio.h>
来源：http://hz.fengsongda.top/gtvbumdbcw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hfpthk.cn/gtaftdnbce.html

[S02] C：变量与格式化输出
来源：http://hz.xingfuxueyuan.xyz/gthdtrwnei.html

int a = 10; printf("%d\n", a);
来源：http://hz.smart0.xyz/gttfqwumob.html

[S03] C：读入整数
来源：http://hz.hnqzz.top/gtluyfsobm.html

int x; scanf("%d", &x);
来源：http://hz.hfpthk.cn/gtbcuxhpys.html

[S04] C：字符串复制
来源：http://hz.gaohongyu789.top/gtbfinxcxs.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yvedp.cn/gtweyapucv.html

[S05] C：字符串长度
来源：http://hz.yj20258.top/gtlyrxuarv.html

strlen(s)
来源：http://hz.bjfxy.top/gtsllwedvf.html

[S06] C：字符串比较
来源：http://hz.quarkkingdee.top/gthowtnubx.html

strcmp(a, b) == 0
来源：http://hz.chenzaomai.com/gtthelfzrg.html

[S07] C：数组遍历求和
来源：http://hz.kuanghao11.cn/gtnxksizku.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.guannengcc.top/gtcynpxcrf.html

[S08] C：动态内存分配与释放
来源：http://hz.nanxinkj.top/gtlikahfyr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.birdmap.top/gtqypokrcu.html

[S09] C：结构体定义与初始化
来源：http://hz.sweek.top/gtxbywvlng.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.shuidangran.top/gtuqcfyyxp.html

[S10] C：指针与解引用
来源：http://hz.guannengcc.top/gtudcofgin.html

int *p = &a;  *p = 5;
来源：http://hz.havefunace.top/gtjmooyrkz.html

[S11] C：逐行读文件
来源：http://hz.ybcxt.top/gtzpdjzymx.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.quarkkingdee.top/gtiuibmadm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.guowangkeji.top/gtzwogzrol.html

fclose(f);
来源：http://hz.zhixingplan.top/gtzyibwpvx.html

[S12] C：写文件
来源：http://hz.hnqzz.top/gtlkwwfjwo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.0kj1m.cn/gtqqggudlf.html

[S13] C：宏定义
来源：http://hz.smart0.xyz/gtmycqvthc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jinqigufen.top/gtgbnpalom.html

[S14] C：枚举
来源：http://hz.dashuyun.cn/gtdgqfrvwj.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.iojbl.cn/gtcciflejn.html

[S15] C：类型转换
来源：http://hz.redwolf501.top/gtqsgkzqtw.html

(double) a / b
来源：http://hz.yanxiufei.cn/gtyjiqobfz.html

[S16] C：位操作置位
来源：http://hz.hnqzz.top/gtdkhufnin.html

x |= (1 << 3);
来源：http://hz.meibo888.top/gtgbldzgcq.html

[S17] C：安全拼接字符串
来源：http://hz.svipenyu.cn/gtlpusoqpx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.iojbl.cn/gttdahwxzv.html

[S18] C：命令行参数
来源：http://hz.daxiang520.top/gtuhdlkxya.html

int main(int argc, char **argv)
来源：http://hz.guannengcc.top/gtjkzsween.html

[S19] C：快速排序
来源：http://hz.yueranfly.top/gtanmqmxpe.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yanxiufei.cn/gtraqlyyhg.html

[S20] C：二分查找
来源：http://hz.316326.xyz/gtagoopqzn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yvedp.cn/gtimuttwvv.html

[S21] C：字符类别判断
来源：http://hz.andypj.xyz/gtnkqejrfc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.daria6918.cn/gtumwbtuap.html

[S22] C：字符串转数字
来源：http://hz.jianghu66.top/gtqzbjrjye.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shangyingyoupin.top/gtnwlgycfz.html

[S23] C：随机数
来源：http://hz.tian-w.cn/gtlpwysrqn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jiagoushi.top/gtvuxzvvzc.html

[S24] C：获取本地时间
来源：http://hz.jiagoushi.top/gttxlpsqmy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.redwolf501.top/gtrimfpjil.html

[S25] C：内存拷贝
来源：http://hz.hnxiangtu.top/gtyvkpuqbv.html

memcpy(dst, src, n);
来源：http://hz.yangfankeji.com/gtuaciqach.html

[S26] C：内存清零
来源：http://hz.gzhubu.top/gtvzcikqug.html

memset(a, 0, sizeof a);
来源：http://hz.vqdsnc.cn/gtnqmhzoog.html

[S27] C：定义常量
来源：http://hz.hysaishi.cn/gtifzapkkr.html

const double PI = 3.14159;
来源：http://hz.ppjwa.cn/gtnbgyutcc.html

[S28] C：静态变量
来源：http://hz.yj20258.top/gtzfmkudcs.html

static int counter = 0;
来源：http://hz.nwbrower.top/gtjhgdbdya.html

[S29] C：变参函数
来源：http://hz.chenlongwang.top/gtejfjihea.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.snrcjt.cn/gtvjuqgmva.html

[S30] C：头文件保护
来源：http://hz.cdnleiting.top/gtsnlqdakr.html

#ifndef X_H
来源：http://hz.dashuyun.cn/gtachxtbqz.html

#define X_H
来源：http://hz.cashguo.top/gtrpraqwpc.html

#endif
来源：http://hz.daria6918.cn/gtqgczhlsg.html

[S31] C++：Hello World
来源：http://hz.gogol.net.cn/gtgjgzelmj.html

#include <iostream>
来源：http://hz.snrcjt.cn/gtffustmrg.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hnxiangtu.top/gtyofleabf.html

[S32] C++：字符串
来源：http://hz.yj20258888.top/gtvwulpdqe.html

std::string s = "hi";  s += "!";
来源：http://hz.yj202588.top/gtqdirwfie.html

[S33] C++：vector 增删
来源：http://hz.shanyushiyangtech.top/gtldcpdwcf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hnxiangtu.top/gtesotdmre.html

[S34] C++：遍历 vector
来源：http://hz.nanxuanxn.top/gtvppkaxdh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ydzc1.top/gtjveeraud.html

[S35] C++：map
来源：http://hz.tianlin.xyz/gtmznuxxlw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.redwolf501.top/gtoofvrsqc.html

[S36] C++：unordered_map
来源：http://hz.52xcode.cn/gthxmlfzbw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cucudq.cn/gtcecprvxg.html

[S37] C++：set
来源：http://hz.jlsjyb.cn/gtkufilanf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hywenlv.cn/gtigqifgkw.html

[S38] C++：排序
来源：http://hz.nanxuanxn.top/gtsyynnjzk.html

std::sort(v.begin(), v.end());
来源：http://hz.ydzc1.top/gtsdtnfxzd.html

[S39] C++：自定义比较器排序
来源：http://hz.jyoumei.cn/gtntvggvzh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gzhubu.top/gtmsnujbzn.html

[S40] C++：查找元素
来源：http://hz.ydjk.org.cn/gtqaiywvgr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xinyue.icu/gteffgvqrq.html

[S41] C++：类与构造函数
来源：http://hz.yj20258888.top/gtedpepylg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.dashuyun.cn/gtaphuqeln.html

[S42] C++：继承与虚函数
来源：http://hz.shanyushiyangkeji.top/gtwmblintt.html

class B : public Base { public: void f() override {} };
来源：http://hz.cqqwz.cn/gtbqacjzos.html

[S43] C++：智能指针
来源：http://hz.zhijiandao.cn/gtajbtftwu.html

auto p = std::make_unique<int>(5);
来源：http://hz.iojbl.cn/gtytnriisu.html

[S44] C++：引用传参
来源：http://hz.gotoacloud.top/gtbwfgacse.html

void inc(int &x) { ++x; }
来源：http://hz.shanyushiyangkeji.top/gtlffgmvdd.html

[S45] C++：lambda
来源：http://hz.0kj1m.cn/gtbtbtuluj.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hfpthk.cn/gttgskkapp.html

[S46] C++：函数模板
来源：http://hz.yanxiufei.cn/gtytjmuskr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jinyuanbaomall.cn/gtsigngtsw.html

[S47] C++：结构化绑定遍历
来源：http://hz.zycfv.cn/gtqzxubynq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.chenzaomai.com/gtzpmknuof.html

[S48] C++：逐行读文件
来源：http://hz.zhiwuduotai.top/gtdsbmljgh.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.birdmap.top/gtueybuoty.html

while (std::getline(in, line)) { }
来源：http://hz.yangfankeji.com/gtxxcwcxil.html

[S49] C++：写文件
来源：http://hz.daria6918.cn/gtrhxsblex.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhijiandao.cn/gtwiblweyo.html

[S50] C++：格式化数字
来源：http://hz.yueranfly.top/gttktyuxpj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hongshengwenyu.top/gtwldbemwe.html

[S51] C++：显式类型转换
来源：http://hz.hnxiangtu.top/gtyfrrzsgh.html

static_cast<double>(a) / b
来源：http://hz.xingfuxueyuan.xyz/gtouwowdwx.html

[S52] C++：const 与 noexcept
来源：http://hz.svipenyu.cn/gtdfamvglg.html

int size() const noexcept { return n_; }
来源：http://hz.yongpay.top/gtcctrfdip.html

[S53] C++：移动语义
来源：http://hz.ppjwa.cn/gtdxtatotn.html

std::vector<int> w = std::move(v);
来源：http://hz.hongshengwenyu.top/gtgbqnzayq.html

[S54] C++：异常处理
来源：http://hz.xuanzx.com/gtzdanczgn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shanyushiyangtech.top/gtabbdgwll.html

[S55] C++：结构化绑定
来源：http://hz.dianchejie.cn/gtdnqrtqqp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.pengpengdd.cyou/gtvfobxbfl.html

[S56] C++：optional
来源：http://hz.hysaishi.cn/gtmvxuknfn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.vqdsnc.cn/gtydztlslc.html

[S57] C++：编译期常量
来源：http://hz.9152youxi.cn/gttpsnlevs.html

constexpr int N = 10;
来源：http://hz.hnqzz.top/gtmrdpvskq.html

[S58] C++：命名空间
来源：http://hz.jyoumei.cn/gtjcyqmtdm.html

namespace ns { int f() { return 1; } }
来源：http://hz.aibaodan.cn/gteteqxpse.html

[S59] C++：静态断言
来源：http://hz.shangyingyoupin.top/gtxvsifhwz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.guannengcc.top/gtsmdxqfdb.html

[S60] C++：遍历并删除元素
来源：http://hz.yonumen.top/gtyyyinbxa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.redwolf501.top/gtdswvwmkb.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtzoczxgzu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.guowangkeji.top/gtbqcfdils.html

================================================================================
来源：http://hz.jinqigfzy.top/gthzuvogoj.html

[T01] Kotlin：Hello World
来源：http://hz.jlsjyb.cn/gtronwyyyk.html

println("Hello")
来源：http://hz.jinghuilouyu.cn/gtjptidfdd.html

[T02] Kotlin：变量
来源：http://hz.c1oappe.top/gtcszmpwrl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.havefunace.top/gtxupfjazf.html

[T03] Kotlin：字符串模板
来源：http://hz.dashuyun.cn/gtqfupfdxr.html

"值: $b"
来源：http://hz.52xcode.cn/gtuhmcxxyj.html

[T04] Kotlin：空安全
来源：http://hz.zhoulong.xyz/gtvnmmgwrx.html

val n: String? = null;  n?.length
来源：http://hz.mhx1999.top/gtcpbkprua.html

[T05] Kotlin：when 表达式
来源：http://hz.jqgfzy.top/gthtglixek.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.snrcjt.cn/gtfhaaafyy.html

[T06] Kotlin：集合映射
来源：http://hz.xylfe.cn/gtqybwoxab.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.bjfxy.top/gttbhgkrai.html

[T07] Kotlin：集合过滤
来源：http://hz.zhoulong.xyz/gtdqfludpr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.chenlongwang.top/gtawmkuezv.html

[T08] Kotlin：数据类
来源：http://hz.zycfv.cn/gtxnyvtioz.html

data class User(val name: String, val age: Int)
来源：http://hz.zdqjudy.top/gtltyryvaw.html

[T09] Kotlin：扩展函数
来源：http://hz.jqgfzy.top/gtpclvdjhc.html

fun String.exclaim() = this + "!"
来源：http://hz.ydjk.org.cn/gtocfkctsl.html

[T10] Kotlin：默认参数
来源：http://hz.ehwqpu.com/gtpmfjylwi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.vqdsnc.cn/gtirxezpuk.html

[T11] Kotlin：协程
来源：http://hz.ywan-chungtsiang.top/gtcslnbsgy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.0kj1m.cn/gthuiknehc.html

[T12] Kotlin：解构声明
来源：http://hz.yanxiufei.cn/gtzwejwoxx.html

val (a, b) = Pair(1, 2)
来源：http://hz.bjfxy.top/gttzuvlpdi.html

[T13] Kotlin：只读 Map
来源：http://hz.yj202588.top/gtfatrrjth.html

val m = mapOf("a" to 1)
来源：http://hz.andypj.xyz/gtvkvfqsak.html

[T14] Kotlin：循环
来源：http://hz.c1oappe.top/gtmvccwsqr.html

for (i in 1..10) println(i)
来源：http://hz.316326.xyz/gtblmvokyy.html

[T15] Kotlin：接口
来源：http://hz.xuanzx.com/gtswdkeath.html

interface Shape { fun area(): Double }
来源：http://hz.yuanzhike.top/gtqqxfsula.html

[T16] Swift：Hello World
来源：http://hz.quarkkingdee.top/gtuudodmcy.html

print("Hello")
来源：http://hz.jqgfzy.top/gtldwfmobx.html


<!-- 参考信息 -->