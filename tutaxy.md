代发 wailian999

[Q80] 字符串截取
来源：http://hz.xziqi.cn/gtgatkekre.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtucnkwfni.html

[Q81] 字符串替换
来源：http://hz.sxryk.cn/gtnevzefrc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ydzc1.top/gttnsojmaj.html

[Q82] 字符长度与字节长度
来源：http://hz.nanxuanxn.top/gtyyuwlsbs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.smart0.xyz/gtprvebumh.html

[Q83] 大小写转换
来源：http://hz.aibaodan.cn/gtvalrbogt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ybcxt.top/gtiidtossz.html

[Q84] 去除首尾空格
来源：http://hz.zycfv.cn/gtleajoroj.html

SELECT TRIM(name) FROM users;
来源：http://hz.pycfn.com/gtvfpmvgpv.html

[Q85] 数值取整
来源：http://hz.yj20258.top/gtlkfukbdy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.gogol.net.cn/gtboeanfyp.html

[Q86] 读取 JSON 字段
来源：http://hz.shuidangran.top/gtpnbctkhr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.cheryme.top/gtymyqsoyf.html

[Q87] JSON 字段做条件
来源：http://hz.shangyingyoupin.top/gtckzmidhd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.guowangkeji.top/gtkwejihza.html

[Q88] 行转列（条件聚合）
来源：http://hz.aibaodan.cn/gtpmqibqao.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yongpay.top/gtdaswxujg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.tanke756.top/gteznevxuz.html

[Q89] 判断表是否存在
来源：http://hz.xziqi.cn/gttvoyutsp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.snrcjt.cn/gthwgcoagg.html

[Q90] 生成序号列
来源：http://hz.xylfe.cn/gtmtccjdsw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cheryme.top/gtyuzskiws.html

================================================================================
来源：http://hz.ydjk.org.cn/gtdbvntfrb.html

R. Bash 专题
来源：http://hz.guowangkeji.top/gtscyjtcdu.html

================================================================================
来源：http://hz.yj202588.top/gtttzigwxs.html

[R01] shebang 与严格模式
来源：http://hz.feifeiyinyue.top/gtlibfheop.html

#!/usr/bin/env bash
来源：http://hz.cqqwz.cn/gtnmrrjazc.html

set -euo pipefail
来源：http://hz.ydzc1.top/gtehrefjgd.html

[R02] 变量赋值与使用
来源：http://hz.chenjidiqi.icu/gtwtokvlnq.html

name="Tom"; echo "$name"
来源：http://hz.gzhubu.top/gtxwqogxzz.html

[R03] 只读变量
来源：http://hz.wangshuangyany.cn/gturndlqox.html

readonly PI=3.14
来源：http://hz.tianlin.xyz/gtndjywqgh.html

[R04] 位置参数
来源：http://hz.jianghu66.top/gtqupafnfl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.meibo888.top/gtqakrplih.html

[R05] 参数默认值
来源：http://hz.jqgfzy.top/gtntblicem.html

name="${1:-default}"
来源：http://hz.xuetiantiany.cn/gtqejpityd.html

[R06] 判断命令是否存在
来源：http://hz.sufxvd.cn/gtrfibvheq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.smart0.xyz/gtlzsnlvlk.html

[R07] if 判断文件
来源：http://hz.zhiwuduotai.top/gtvmbnekwo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jinqigfzy.top/gtlwsafmoe.html

[R08] 数值比较
来源：http://hz.svipenyu.cn/gtzpakeqql.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jyoumei.cn/gtqfpmiqek.html

[R09] 字符串比较
来源：http://hz.ivvv.top/gtmpewlvrg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jyoumei.cn/gtolzgsgom.html

[R10] 正则匹配
来源：http://hz.316326.xyz/gtivarsplw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yuxming.cn/gtghdxjlkl.html

[R11] case 多分支
来源：http://hz.hongshengwenyu.top/gtehvzwufi.html

case "$1" in
来源：http://hz.zhixingplan.top/gtyynjjlrp.html

start) echo "启动" ;;
来源：http://hz.tian-w.cn/gtacgnevro.html

stop)  echo "停止" ;;
来源：http://hz.yanxiufei.cn/gtvoqirfby.html

*)     echo "未知命令" ;;
来源：http://hz.nanxinkj.top/gtitienooe.html

esac
来源：http://hz.yongpay.top/gtpurcldmk.html

[R12] for 遍历文件
来源：http://hz.ydzc1.top/gtzqkpkxip.html

for f in *.txt; do echo "$f"; done
来源：http://hz.quarkkingdee.top/gtutwkyisy.html

[R13] for 计数循环
来源：http://hz.chenjidiqi.icu/gtjqnttnqs.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.nanxinkj.top/gtvmpucfyy.html

[R14] C 风格 for
来源：http://hz.sxryk.cn/gtlnwrlitu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hnxiangtu.top/gtriuxxzqc.html

[R15] while 逐行读文件
来源：http://hz.fengsongda.top/gtatepfwdh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.nanxinkj.top/gtioimqwbs.html

[R16] until 等待条件
来源：http://hz.yuanzhike.top/gtqcpmcnju.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.aizwys.cn/gtxytuyvjb.html

[R17] 数组定义与取值
来源：http://hz.yvedp.cn/gtbzbsvmfs.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.smart0.xyz/gtoytqaucd.html

[R18] 遍历数组
来源：http://hz.cdnleiting.top/gtaxwuiawo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.feifeiyinyue.top/gtjbvcyxvm.html

[R19] 数组长度
来源：http://hz.yanxiufei.cn/gtcdkgresy.html

echo "${#arr[@]}"
来源：http://hz.birdmap.top/gtyzcuyyul.html

[R20] 关联数组（字典）
来源：http://hz.birdmap.top/gthzvwihly.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.sysykeji.top/gtlfjoffkw.html

[R21] 字符串长度
来源：http://hz.hongshengwenyu.top/gtoxgffemb.html

echo "${#s}"
来源：http://hz.aizwys.cn/gttbdefihk.html

[R22] 截取子串
来源：http://hz.zhijiandao.cn/gtetvtjlvw.html

echo "${s:0:5}"
来源：http://hz.hnxiangtu.top/gthajcjyur.html

[R23] 字符串替换
来源：http://hz.jlsjyb.cn/gtqrsteyfb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shuidangran.top/gtlwhwmgik.html

[R24] 大小写转换
来源：http://hz.feifeiyinyue.top/gtahfzjiuc.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xziqi.cn/gtkwptdknz.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhixingplan.top/gtrkkdeqvt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yj20258888.top/gtoadsdqxd.html

[R26] 命令替换
来源：http://hz.pengpengdd.cyou/gtfuhupoeh.html

now=$(date +%F); echo "$now"
来源：http://hz.ydzc1.top/gtucjqovxy.html

[R27] 算术展开
来源：http://hz.shanyushiyangtech.top/gtfswbtibe.html

echo $((1 + 2 * 3))
来源：http://hz.aizwys.cn/gtzxhdsoef.html

[R28] 浮点运算
来源：http://hz.sweek.top/gtcxkmbjez.html

echo "scale=2; 10/3" | bc
来源：http://hz.yangfankeji.com/gtkftjsjpg.html

[R29] 定义函数
来源：http://hz.nwbrower.top/gttrxuytbv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.redwolf501.top/gtxsocgrzv.html

[R30] 函数返回状态码
来源：http://hz.gaohongyu789.top/gtdhalnmlv.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.svipenyu.cn/gtyfaucfom.html

[R31] 局部变量
来源：http://hz.zhongyouzk.top/gtjordxzhj.html

f() { local x=1; echo "$x"; }
来源：http://hz.sysykeji.top/gtyjcmjwmt.html

[R32] 参数个数校验
来源：http://hz.havefunace.top/gtychfcepp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.dashuyun.cn/gthzskpxti.html

[R33] 捕获错误并提示行号
来源：http://hz.gaohongyu789.top/gtxfdczknt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhixingplan.top/gtlavifygq.html

[R34] 退出时清理
来源：http://hz.jqgufenzy.top/gtvdgvccqc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hysaishi.cn/gtfhhkaoly.html

[R35] 后台执行并等待
来源：http://hz.xinyue.icu/gtlcciqtwz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.bjfxy.top/gtiqoqztzr.html

[R36] 并发执行多个任务
来源：http://hz.nanxinkj.top/gtncyphlav.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shangyingyoupin.top/gtnbalxlix.html

[R37] 把输出赋给变量
来源：http://hz.shuidangran.top/gtzyikamof.html

files=$(ls -1)
来源：http://hz.gotoacloud.top/gtzdxorrrg.html

[R38] 管道串联
来源：http://hz.ydjk.org.cn/gtjftayomf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hywenlv.cn/gtdrwgbzie.html

[R39] 重定向标准输出与错误
来源：http://hz.shuidangran.top/gtenllfgqi.html

cmd > out.log 2>&1
来源：http://hz.sweek.top/gtxuzpbsqq.html

[R40] 追加写日志
来源：http://hz.zycfv.cn/gtwnhaugpe.html

echo "log" >> out.log
来源：http://hz.hongshengwenyu.top/gtwirrvatw.html

[R41] 丢弃输出
来源：http://hz.yanxiufei.cn/gtwcpjyiof.html

cmd >/dev/null 2>&1
来源：http://hz.shanyushiyangtech.top/gtneqdltox.html

[R42] 输入重定向
来源：http://hz.cucudq.cn/gtcwbnqnix.html

wc -l < a.txt
来源：http://hz.tianlin.xyz/gtdcsjyslj.html

[R43] 按名字查找文件
来源：http://hz.gogol.net.cn/gtdqqeiwgx.html

find . -name "*.log" -type f
来源：http://hz.cheryme.top/gtlqgejvae.html

[R44] 按修改时间查找
来源：http://hz.ydzc1.top/gteevzoamx.html

find . -mtime -7 -type f
来源：http://hz.wangdashe.top/gtdnniuqww.html

[R45] 批量删除
来源：http://hz.shanyushiyangtech.top/gtoigedvvm.html

find . -name "*.tmp" -delete
来源：http://hz.gogol.net.cn/gtnfrkbjtk.html

[R46] 递归替换文件内容
来源：http://hz.andypj.xyz/gtqnybiqud.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jinghuilouyu.cn/gtvvraoukk.html

[R47] sed 单行替换
来源：http://hz.sysykeji.top/gtqitczutf.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ywan-chungtsiang.top/gtygljcblf.html

[R48] awk 取指定列
来源：http://hz.kuanghao11.cn/gtjsnlmjzb.html

awk '{print $1, $3}' a.txt
来源：http://hz.yuanzhike.top/gtyjzjkpqc.html

[R49] awk 带条件
来源：http://hz.wangshuangyany.cn/gtztmyhdrz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cdnleiting.top/gtsarpkbxd.html

[R50] awk 求和
来源：http://hz.xinyue.icu/gtnkxndvfq.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ydzc1.top/gtyiskqznh.html

[R51] 排序去重取前几
来源：http://hz.yangfankeji.com/gttimqdiin.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.52xcode.cn/gtejlvkqlz.html

[R52] 统计行数
来源：http://hz.nanxuanxn.top/gthwjazcus.html

wc -l a.txt
来源：http://hz.pycfn.com/gtxnrjzbyj.html

[R53] 查看文件头与实时尾
来源：http://hz.ydjk.org.cn/gtjqytubzd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.sweek.top/gtbeltfkri.html

[R54] 比较两个文件
来源：http://hz.yongpay.top/gtduvhvulv.html

diff a.txt b.txt
来源：http://hz.xuanzx.com/gtfqftoihe.html

[R55] 压缩与解压
来源：http://hz.yvedp.cn/gtmzbvnegb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zycfv.cn/gtrrnmtara.html

[R56] 远程拷贝
来源：http://hz.jiagoushi.top/gtnkwibpiw.html

scp file user@host:/path/
来源：http://hz.chenjidiqi.icu/gtejhdnvqn.html

[R57] 远程执行命令
来源：http://hz.aibaodan.cn/gtayhlkvxi.html

ssh user@host 'uptime'
来源：http://hz.dianchejie.cn/gtdhrjtghj.html

[R58] 下载文件
来源：http://hz.zhongyouzk.top/gtypucepxc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.nanxinkj.top/gtihchtkiy.html

[R59] 发 POST JSON
来源：http://hz.yongpay.top/gtncnjphfi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhijiandao.cn/gtvynupfyz.html

[R60] 只看 HTTP 状态码
来源：http://hz.guannengcc.top/gteaflmvil.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.tianlin.xyz/gtpqwtgiiv.html

[R61] 磁盘占用
来源：http://hz.aibaodan.cn/gtkexscfqg.html

df -h;  du -sh *
来源：http://hz.jqgfzy.top/gtzlucnimv.html

[R62] 找最占空间的文件
来源：http://hz.0kj1m.cn/gttvnbyisx.html

du -ah . | sort -rh | head -10
来源：http://hz.dianchejie.cn/gtagvfbuoi.html

[R63] 内存与进程
来源：http://hz.haohaochexian.top/gtoqwitlrh.html

free -h;  ps aux | grep nginx
来源：http://hz.hysaishi.cn/gtoddukgzn.html

[R64] 结束进程
来源：http://hz.zhijiandao.cn/gtkbhfgtyp.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sysykeji.top/gtjaoeegwa.html

[R65] 查看端口占用
来源：http://hz.iojbl.cn/gtbuizeiud.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.iojbl.cn/gtxavqotwc.html

[R66] 定时任务
来源：http://hz.hammf.cn/gtrvesgtzp.html

crontab -e;  crontab -l
来源：http://hz.tianlin.xyz/gtievgonpm.html

[R67] 生成随机十六进制串
来源：http://hz.c1oappe.top/gtrpoxnrei.html

openssl rand -hex 16
来源：http://hz.meibo888.top/gtukwownap.html

[R68] 计算文件校验值
来源：http://hz.kuanghao11.cn/gtsyqywule.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cqqwz.cn/gtjrennwkk.html

[R69] 生成随机密码
来源：http://hz.xinyue.icu/gtdobsvgqm.html

head -c 16 /dev/urandom | base64
来源：http://hz.shanyushiyangtech.top/gtqpeyimni.html

[R70] 时间戳与互转
来源：http://hz.tian-w.cn/gtgunjuoyl.html

date +%s;  date -d @1700000000
来源：http://hz.zdqjudy.top/gtnwvqmhjf.html

[R71] 日期格式化
来源：http://hz.guowangkeji.top/gtqcblheiv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gzhubu.top/gtqqpaiqnd.html

[R72] 等待端口就绪
来源：http://hz.hnxiangtu.top/gtmzrhidwg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.bjfxy.top/gtnwefxfft.html

[R73] 分割大日志
来源：http://hz.ivvv.top/gtevbzdkpz.html

split -l 1000 big.log part_
来源：http://hz.zhiwuduotai.top/gtzjhkfdgf.html

[R74] 批量重命名
来源：http://hz.sweek.top/gtctcidgzq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.pycfn.com/gtrvpknonb.html

[R75] 导出环境变量
来源：http://hz.birdmap.top/gtpctlnezs.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xziqi.cn/gtlfmwztdm.html

[R76] 使用临时文件
来源：http://hz.kuanghao11.cn/gtjlpkqbzz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jqgfzy.top/gtxdflphwp.html

[R77] 读取用户输入
来源：http://hz.jlsjyb.cn/gtmxkpmwaj.html

read -rp "请输入: " ans
来源：http://hz.jlsjyb.cn/gtcpepnicv.html

[R78] 交互式菜单
来源：http://hz.jinghuilouyu.cn/gttjdllryu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hfpthk.cn/gtrdobjltf.html

[R79] 解析命令行选项
来源：http://hz.cashguo.top/gtmkatqxaq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jinyuanbaomall.cn/gtduenarxp.html

[R80] 查看脚本执行耗时
来源：http://hz.cheryme.top/gtudpqmjat.html

time ./run.sh
来源：http://hz.svipenyu.cn/gtcyazkask.html

================================================================================
来源：http://hz.fzhhl.top/gtrhzbdwsf.html

S. C / C++ 专题
来源：http://hz.chenzaomai.com/gthbfxrjuy.html

================================================================================
来源：http://hz.cheryme.top/gtdyhpbjhw.html

[S01] C：Hello World
来源：http://hz.0kj1m.cn/gtslkftxob.html

#include <stdio.h>
来源：http://hz.fengsongda.top/gtnhwexpur.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ydjk.org.cn/gtjmexdqjz.html

[S02] C：变量与格式化输出
来源：http://hz.haohaochexian.top/gtijoyturk.html

int a = 10; printf("%d\n", a);
来源：http://hz.tian-w.cn/gtncdgetdp.html

[S03] C：读入整数
来源：http://hz.chenzaomai.com/gttxvaocur.html

int x; scanf("%d", &x);
来源：http://hz.wangdashe.top/gtbihnrmlh.html

[S04] C：字符串复制
来源：http://hz.gotoacloud.top/gtatikaxen.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.bjfxy.top/gtcqkybate.html

[S05] C：字符串长度
来源：http://hz.jqgufenzy.top/gtqdjjhhvu.html

strlen(s)
来源：http://hz.wangdashe.top/gtnnrhoixh.html

[S06] C：字符串比较
来源：http://hz.jinyuanbaomall.cn/gtjbjvvvar.html

strcmp(a, b) == 0
来源：http://hz.hysaishi.cn/gtprjhmgtc.html

[S07] C：数组遍历求和
来源：http://hz.zhengqikj.top/gtrfezlrct.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.chenjidiqi.icu/gtuibntnwl.html

[S08] C：动态内存分配与释放
来源：http://hz.0kj1m.cn/gtcjryqlir.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jlsjyb.cn/gthsjxkkuw.html

[S09] C：结构体定义与初始化
来源：http://hz.hnxiangtu.top/gtxqgmccam.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cashguo.top/gtdknahfpl.html

[S10] C：指针与解引用
来源：http://hz.ehwqpu.com/gtdmhjmhyl.html

int *p = &a;  *p = 5;
来源：http://hz.zhijiandao.cn/gtrzlkfbqf.html

[S11] C：逐行读文件
来源：http://hz.yj20258.top/gtancaivnx.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.iojbl.cn/gtkpfatbin.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.52xcode.cn/gtwkplwxyf.html

fclose(f);
来源：http://hz.ydzc1.top/gtfbumnaax.html

[S12] C：写文件
来源：http://hz.feifeiyinyue.top/gtasulryky.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yj202588.top/gtdtdbqxug.html

[S13] C：宏定义
来源：http://hz.hammf.cn/gtdhkahvsi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ydzc1.top/gtcjleybau.html

[S14] C：枚举
来源：http://hz.smart0.xyz/gtxwlmoyzk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jiagoushi.top/gtqnlvvvdv.html

[S15] C：类型转换
来源：http://hz.wangdashe.top/gtrixjbyem.html

(double) a / b
来源：http://hz.xziqi.cn/gtkkemvnus.html

[S16] C：位操作置位
来源：http://hz.cdnleiting.top/gtfwbcqgbp.html

x |= (1 << 3);
来源：http://hz.yanxiufei.cn/gtcoccfomh.html

[S17] C：安全拼接字符串
来源：http://hz.jqgfzy.top/gtaeqvfpve.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.aizwys.cn/gtjorvjgtr.html

[S18] C：命令行参数
来源：http://hz.aizwys.cn/gtlcxpwebs.html

int main(int argc, char **argv)
来源：http://hz.snrcjt.cn/gtuduiobvm.html

[S19] C：快速排序
来源：http://hz.haohaochexian.top/gtzsgxgxgu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jinghuilouyu.cn/gtcnphhmqx.html

[S20] C：二分查找
来源：http://hz.bjfxy.top/gtahhqynvu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.gotoacloud.top/gtodkdtmcc.html

[S21] C：字符类别判断
来源：http://hz.tianlin.xyz/gtckjavbzw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhiwuduotai.top/gtbodctwau.html

[S22] C：字符串转数字
来源：http://hz.yuxming.cn/gteqxjlqkk.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.pycfn.com/gtuoehkamz.html

[S23] C：随机数
来源：http://hz.havefunace.top/gtrwmxrviu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ivvv.top/gtznzpvuaq.html

[S24] C：获取本地时间
来源：http://hz.shzxlz.cn/gtdveygkei.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.bjfxy.top/gtgknffzdi.html

[S25] C：内存拷贝
来源：http://hz.ybcxt.top/gthuqmwvyo.html

memcpy(dst, src, n);
来源：http://hz.jinqigfzy.top/gtsjevgkbi.html

[S26] C：内存清零
来源：http://hz.zycfv.cn/gtdtapcryi.html

memset(a, 0, sizeof a);
来源：http://hz.ywan-chungtsiang.top/gtxtbaixdf.html

[S27] C：定义常量
来源：http://hz.chenlongwang.top/gtpmzxdncp.html

const double PI = 3.14159;
来源：http://hz.xuetiantiany.cn/gtzomntmlg.html

[S28] C：静态变量
来源：http://hz.jqgfzy.top/gtkxydwizs.html

static int counter = 0;
来源：http://hz.yuanzhike.top/gtvexjsevp.html

[S29] C：变参函数
来源：http://hz.redwolf501.top/gtoybakbgs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yanxiufei.cn/gtmoazdgkw.html

[S30] C：头文件保护
来源：http://hz.sweek.top/gtilztjtig.html

#ifndef X_H
来源：http://hz.52xcode.cn/gtqdhnlfvk.html

#define X_H
来源：http://hz.tian-w.cn/gtjtmuxnez.html

#endif
来源：http://hz.zdqjudy.top/gtaolzgnio.html

[S31] C++：Hello World
来源：http://hz.dianchejie.cn/gtnjjpmruo.html

#include <iostream>
来源：http://hz.jinqigfzy.top/gtjnftvagh.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shangyingyoupin.top/gtveybmhvx.html

[S32] C++：字符串
来源：http://hz.daxiang520.top/gtgnsezkjr.html

std::string s = "hi";  s += "!";
来源：http://hz.tianlin.xyz/gtnzjsxkcu.html

[S33] C++：vector 增删
来源：http://hz.yj20258.top/gtoonkvour.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hnxiangtu.top/gtkpvgepms.html

[S34] C++：遍历 vector
来源：http://hz.smart0.xyz/gtxdzcfiuo.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.fzhhl.top/gttqbcapky.html

[S35] C++：map
来源：http://hz.havefunace.top/gtazseumpe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pycfn.com/gtvcvfyubd.html

[S36] C++：unordered_map
来源：http://hz.yj20258.top/gtsifbgqmu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.snrcjt.cn/gtvhlmqjnd.html

[S37] C++：set
来源：http://hz.xylfe.cn/gtepgttqzv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.tanke756.top/gtlxnnxtoi.html

[S38] C++：排序
来源：http://hz.chenjidiqi.icu/gtnaemihfc.html

std::sort(v.begin(), v.end());
来源：http://hz.jinqigfzy.top/gtriljxfma.html

[S39] C++：自定义比较器排序
来源：http://hz.mhx1999.top/gtphvvyzkz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.52xcode.cn/gtqposoore.html

[S40] C++：查找元素
来源：http://hz.52xcode.cn/gtcrothoxd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hfpthk.cn/gtwnexextk.html

[S41] C++：类与构造函数
来源：http://hz.ehwqpu.com/gtmuwpyxna.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.shanyushiyangtech.top/gttyrbekcj.html

[S42] C++：继承与虚函数
来源：http://hz.xinyue.icu/gtzfgswsns.html

class B : public Base { public: void f() override {} };
来源：http://hz.ybcxt.top/gtawurotlt.html

[S43] C++：智能指针
来源：http://hz.zhiwuduotai.top/gtkasiiult.html

auto p = std::make_unique<int>(5);
来源：http://hz.andypj.xyz/gtpauxnkqs.html

[S44] C++：引用传参
来源：http://hz.hnxiangtu.top/gtceptwtef.html

void inc(int &x) { ++x; }
来源：http://hz.hywenlv.cn/gteyotoqgo.html

[S45] C++：lambda
来源：http://hz.yj20258.top/gtsbyvkpuy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinqigufen.top/gtatvrdthh.html

[S46] C++：函数模板
来源：http://hz.smart0.xyz/gtzbamuvrq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.sweek.top/gtrycamheg.html

[S47] C++：结构化绑定遍历
来源：http://hz.cucudq.cn/gtcxdytyja.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zycfv.cn/gtxniuydmu.html

[S48] C++：逐行读文件
来源：http://hz.shuidangran.top/gtgghvdame.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shuidangran.top/gtfaliuryp.html

while (std::getline(in, line)) { }
来源：http://hz.hnqzz.top/gtualngxcr.html

[S49] C++：写文件
来源：http://hz.52xcode.cn/gtnyxrcnqy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jlsjyb.cn/gtcayqkoij.html

[S50] C++：格式化数字
来源：http://hz.xuetiantiany.cn/gtktoaacla.html


<!-- 参考信息 -->