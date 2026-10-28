代发 wailian999

[Q76] 按天统计
来源：http://hz.redwolf501.top/gtfxlwmdxo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.daxiang520.top/gtkhygwxgz.html

[Q77] 时间加减
来源：http://hz.shangyingyoupin.top/gtzrmcxwkz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jinqigufen.top/gtxryrwwyy.html

[Q78] 当前时间
来源：http://hz.birdmap.top/gthuqbqrhg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.andypj.xyz/gtxnmmraix.html

[Q79] 字符串拼接
来源：http://hz.hnqzz.top/gtwmwfiiqi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.guannengcc.top/gtkmxgacdt.html

[Q80] 字符串截取
来源：http://hz.shangyingyoupin.top/gtskawpryd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.havefunace.top/gttozpaiqm.html

[Q81] 字符串替换
来源：http://hz.zhoulong.xyz/gtkaxunduu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jinghuilouyu.cn/gtarnhkphc.html

[Q82] 字符长度与字节长度
来源：http://hz.jinqigfzy.top/gtzaidhpdi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yuanzhike.top/gtkuacdiba.html

[Q83] 大小写转换
来源：http://hz.birdmap.top/gtwzqcavjb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hfpthk.cn/gtpzlozswk.html

[Q84] 去除首尾空格
来源：http://hz.bjfxy.top/gtdtamjbzm.html

SELECT TRIM(name) FROM users;
来源：http://hz.pycfn.com/gtjsshufsm.html

[Q85] 数值取整
来源：http://hz.sweek.top/gtlhbryjlh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hnqzz.top/gtwuvtgucq.html

[Q86] 读取 JSON 字段
来源：http://hz.9152youxi.cn/gtbrqzrxgx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.fengsongda.top/gtbpbuwpbu.html

[Q87] JSON 字段做条件
来源：http://hz.xingfuxueyuan.xyz/gttwbasmce.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yj20258888.top/gtjrlxjwua.html

[Q88] 行转列（条件聚合）
来源：http://hz.hysaishi.cn/gtvzetqlna.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xuetiantiany.cn/gtffpjnvdo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.quarkkingdee.top/gtfuvkonsr.html

[Q89] 判断表是否存在
来源：http://hz.redwolf501.top/gthuvuimcy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhongyouzk.top/gtctpxtbyb.html

[Q90] 生成序号列
来源：http://hz.shuidangran.top/gtsoxqaohc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hnqzz.top/gtbxpvgebb.html

================================================================================
来源：http://hz.andypj.xyz/gtpbuglpiw.html

R. Bash 专题
来源：http://hz.jinqigufen.top/gtcqlrgcfg.html

================================================================================
来源：http://hz.sysykeji.top/gtvmcqwouj.html

[R01] shebang 与严格模式
来源：http://hz.xingfuxueyuan.xyz/gtcrdweefz.html

#!/usr/bin/env bash
来源：http://hz.gzhubu.top/gtkmsakwfp.html

set -euo pipefail
来源：http://hz.daria6918.cn/gtfqstlxti.html

[R02] 变量赋值与使用
来源：http://hz.pengpengdd.cyou/gtmywopkrg.html

name="Tom"; echo "$name"
来源：http://hz.aibaodan.cn/gtkrpgkqgo.html

[R03] 只读变量
来源：http://hz.pengpengdd.cyou/gtawozpuqy.html

readonly PI=3.14
来源：http://hz.zycfv.cn/gtcnrejawb.html

[R04] 位置参数
来源：http://hz.yj202588.top/gtukuoxatr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhixingplan.top/gtjpgmttcn.html

[R05] 参数默认值
来源：http://hz.xuetiantiany.cn/gtzdofzirz.html

name="${1:-default}"
来源：http://hz.hongshengwenyu.top/gturistdco.html

[R06] 判断命令是否存在
来源：http://hz.jinyuanbaomall.cn/gtdshrrfli.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xingfuxueyuan.xyz/gtwdooxmku.html

[R07] if 判断文件
来源：http://hz.yueranfly.top/gtylinngts.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yangfankeji.com/gtqnapsftm.html

[R08] 数值比较
来源：http://hz.tianlin.xyz/gtuhysjyyo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ywan-chungtsiang.top/gtgljgtllo.html

[R09] 字符串比较
来源：http://hz.ydjk.org.cn/gtuagvijny.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.feifeiyinyue.top/gtbyuoedqf.html

[R10] 正则匹配
来源：http://hz.gogol.net.cn/gtanlskvsj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.chenzaomai.com/gtzxiqnblz.html

[R11] case 多分支
来源：http://hz.shzxlz.cn/gtmazlaaeq.html

case "$1" in
来源：http://hz.aibaodan.cn/gtkbhgnczy.html

start) echo "启动" ;;
来源：http://hz.jianghu66.top/gtsdtttsjy.html

stop)  echo "停止" ;;
来源：http://hz.gogol.net.cn/gthskjefab.html

*)     echo "未知命令" ;;
来源：http://hz.shanyushiyangkeji.top/gtdpupiewy.html

esac
来源：http://hz.andypj.xyz/gtqroeyzct.html

[R12] for 遍历文件
来源：http://hz.zdqjudy.top/gtfylqgbrr.html

for f in *.txt; do echo "$f"; done
来源：http://hz.316326.xyz/gtnnwgqdho.html

[R13] for 计数循环
来源：http://hz.guannengcc.top/gtuyuwlcmx.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhoulong.xyz/gttnnbabol.html

[R14] C 风格 for
来源：http://hz.yuanzhike.top/gthbneiqxy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.chenlongwang.top/gtmkjsxxvz.html

[R15] while 逐行读文件
来源：http://hz.ppjwa.cn/gtdxtmgcni.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.guowangkeji.top/gtyudgdqny.html

[R16] until 等待条件
来源：http://hz.zhijiandao.cn/gtxvjjgkhn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zdqjudy.top/gtupdbvqqz.html

[R17] 数组定义与取值
来源：http://hz.yueranfly.top/gtpjhybbbz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.gaohongyu789.top/gtedxeagkj.html

[R18] 遍历数组
来源：http://hz.hongshengwenyu.top/gtyctpqoaw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhengqikj.top/gtfnvmzrwr.html

[R19] 数组长度
来源：http://hz.feifeiyinyue.top/gtnitjbzpo.html

echo "${#arr[@]}"
来源：http://hz.shanyushiyangtech.top/gtezaoutvy.html

[R20] 关联数组（字典）
来源：http://hz.havefunace.top/gtnucormqm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.gotoacloud.top/gtopupvnez.html

[R21] 字符串长度
来源：http://hz.nanxuanxn.top/gtlzucmbir.html

echo "${#s}"
来源：http://hz.jinghuilouyu.cn/gtyxydmdrs.html

[R22] 截取子串
来源：http://hz.316326.xyz/gtayiwvqov.html

echo "${s:0:5}"
来源：http://hz.52xcode.cn/gtbkwiwkvb.html

[R23] 字符串替换
来源：http://hz.c1oappe.top/gtfnbwkyky.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.dashuyun.cn/gttcrjhrus.html

[R24] 大小写转换
来源：http://hz.xuanzx.com/gtgksudkmk.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.gzhubu.top/gtdovbsxtz.html

[R25] 去后缀 / 去前缀
来源：http://hz.dianchejie.cn/gtxnzjuxhs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.smart0.xyz/gtenigqtva.html

[R26] 命令替换
来源：http://hz.xylfe.cn/gtowqgvmde.html

now=$(date +%F); echo "$now"
来源：http://hz.shanyushiyangkeji.top/gtougoukwh.html

[R27] 算术展开
来源：http://hz.zycfv.cn/gtqqekwpfe.html

echo $((1 + 2 * 3))
来源：http://hz.sweek.top/gtwuizbuup.html

[R28] 浮点运算
来源：http://hz.andypj.xyz/gtgbbxvebl.html

echo "scale=2; 10/3" | bc
来源：http://hz.9152youxi.cn/gtenkwxwyf.html

[R29] 定义函数
来源：http://hz.yj20258.top/gtnmowyhcz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.chenzaomai.com/gtxbgajngb.html

[R30] 函数返回状态码
来源：http://hz.yanxiufei.cn/gtoogvqjcu.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gogol.net.cn/gtdsuyonbc.html

[R31] 局部变量
来源：http://hz.andypj.xyz/gtfjweqxva.html

f() { local x=1; echo "$x"; }
来源：http://hz.yonumen.top/gtcqjyuuey.html

[R32] 参数个数校验
来源：http://hz.jlsjyb.cn/gtzybnzixy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xuetiantiany.cn/gtlntogory.html

[R33] 捕获错误并提示行号
来源：http://hz.zhengqikj.top/gtrgvokaee.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.52xcode.cn/gtuurzocls.html

[R34] 退出时清理
来源：http://hz.jinqigufen.top/gtbeftjywj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.wangshuangyany.cn/gtssyeuukr.html

[R35] 后台执行并等待
来源：http://hz.aibaodan.cn/gtlksdyiiv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jinyuanbaomall.cn/gthhdyuqmu.html

[R36] 并发执行多个任务
来源：http://hz.zdqjudy.top/gtuwwhxlvq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yvedp.cn/gtviouylhu.html

[R37] 把输出赋给变量
来源：http://hz.ybcxt.top/gtcjdlrgju.html

files=$(ls -1)
来源：http://hz.yanxiufei.cn/gthmevucjh.html

[R38] 管道串联
来源：http://hz.nanxinkj.top/gtjbtvolem.html

cat a.txt | grep -i error | wc -l
来源：http://hz.aizwys.cn/gtglyafkyy.html

[R39] 重定向标准输出与错误
来源：http://hz.hnqzz.top/gtxurntsxs.html

cmd > out.log 2>&1
来源：http://hz.xziqi.cn/gtkfeerxbo.html

[R40] 追加写日志
来源：http://hz.316326.xyz/gtelszqhdl.html

echo "log" >> out.log
来源：http://hz.jqgfzy.top/gtygwdmxvl.html

[R41] 丢弃输出
来源：http://hz.cucudq.cn/gtmknjzqli.html

cmd >/dev/null 2>&1
来源：http://hz.chenzaomai.com/gtngtpyyvd.html

[R42] 输入重定向
来源：http://hz.quarkkingdee.top/gtthpvvrad.html

wc -l < a.txt
来源：http://hz.bjfxy.top/gtvdhxojfh.html

[R43] 按名字查找文件
来源：http://hz.zhijiandao.cn/gtquueegqj.html

find . -name "*.log" -type f
来源：http://hz.gotoacloud.top/gtdjsiufqn.html

[R44] 按修改时间查找
来源：http://hz.gaohongyu789.top/gthgrzdveb.html

find . -mtime -7 -type f
来源：http://hz.0kj1m.cn/gtnkqrlokz.html

[R45] 批量删除
来源：http://hz.vqdsnc.cn/gtqpwtqpcu.html

find . -name "*.tmp" -delete
来源：http://hz.tian-w.cn/gtqpeuiedo.html

[R46] 递归替换文件内容
来源：http://hz.sweek.top/gtqwxddxhq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.dashuyun.cn/gtwkavqnjh.html

[R47] sed 单行替换
来源：http://hz.hysaishi.cn/gtfcfssrws.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hongshengwenyu.top/gthmqpionw.html

[R48] awk 取指定列
来源：http://hz.dianchejie.cn/gtgzccedvt.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhoulong.xyz/gtakenyoeh.html

[R49] awk 带条件
来源：http://hz.cucudq.cn/gtavjsssbv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhoulong.xyz/gtpxtowcaw.html

[R50] awk 求和
来源：http://hz.yuanzhike.top/gtfnyimjud.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.birdmap.top/gtmonmyggh.html

[R51] 排序去重取前几
来源：http://hz.guowangkeji.top/gtkoqgeprz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jqgfzy.top/gtroaketax.html

[R52] 统计行数
来源：http://hz.yanxiufei.cn/gtnboyxves.html

wc -l a.txt
来源：http://hz.havefunace.top/gtehknkpmq.html

[R53] 查看文件头与实时尾
来源：http://hz.shuidangran.top/gtvbcakwln.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cucudq.cn/gtoroqfbqw.html

[R54] 比较两个文件
来源：http://hz.shangyingyoupin.top/gtvokjafei.html

diff a.txt b.txt
来源：http://hz.zhijiandao.cn/gtkuolmdii.html

[R55] 压缩与解压
来源：http://hz.jinyuanbaomall.cn/gtbrneqozf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cqqwz.cn/gtczlqwhzf.html

[R56] 远程拷贝
来源：http://hz.chenlongwang.top/gtrcrxvtfe.html

scp file user@host:/path/
来源：http://hz.bjfxy.top/gtpoxmmoef.html

[R57] 远程执行命令
来源：http://hz.yj20258888.top/gtvfpkomlt.html

ssh user@host 'uptime'
来源：http://hz.xingfuxueyuan.xyz/gtjrqejgys.html

[R58] 下载文件
来源：http://hz.snrcjt.cn/gtapxcqnfb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ybcxt.top/gtkqjlzbgx.html

[R59] 发 POST JSON
来源：http://hz.jlsjyb.cn/gtsxrquvvz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.sufxvd.cn/gtxofkeqow.html

[R60] 只看 HTTP 状态码
来源：http://hz.xingfuxueyuan.xyz/gtrhgshmyn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yuxming.cn/gtltqxnore.html

[R61] 磁盘占用
来源：http://hz.jinqigufen.top/gtyvxvjexb.html

df -h;  du -sh *
来源：http://hz.hywenlv.cn/gtxjxzlxnl.html

[R62] 找最占空间的文件
来源：http://hz.gaohongyu789.top/gthabwplbn.html

du -ah . | sort -rh | head -10
来源：http://hz.chenzaomai.com/gtmmyqerwz.html

[R63] 内存与进程
来源：http://hz.ywan-chungtsiang.top/gtycevifir.html

free -h;  ps aux | grep nginx
来源：http://hz.guowangkeji.top/gtzigvalei.html

[R64] 结束进程
来源：http://hz.yuxming.cn/gtgsibqiwj.html

kill -9 $(pgrep -f app.py)
来源：http://hz.gotoacloud.top/gtzpaozrnh.html

[R65] 查看端口占用
来源：http://hz.cdnleiting.top/gtedyqswnm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xuetiantiany.cn/gtdosfryxq.html

[R66] 定时任务
来源：http://hz.pycfn.com/gtzbehvdbk.html

crontab -e;  crontab -l
来源：http://hz.sweek.top/gtjapiffwm.html

[R67] 生成随机十六进制串
来源：http://hz.jianghu66.top/gteruspycu.html

openssl rand -hex 16
来源：http://hz.yangfankeji.com/gtqjyvcmrv.html

[R68] 计算文件校验值
来源：http://hz.iojbl.cn/gtuzhgvmpd.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xinyue.icu/gtvserhwjg.html

[R69] 生成随机密码
来源：http://hz.bjfxy.top/gtcubfgoqx.html

head -c 16 /dev/urandom | base64
来源：http://hz.ydjk.org.cn/gtqifrezdz.html

[R70] 时间戳与互转
来源：http://hz.ywan-chungtsiang.top/gtzycbmvni.html

date +%s;  date -d @1700000000
来源：http://hz.jqgfzy.top/gtsupivmqv.html

[R71] 日期格式化
来源：http://hz.zhaomingkeji.xyz/gtlsecsbxo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhengqikj.top/gtwkzybiol.html

[R72] 等待端口就绪
来源：http://hz.ehwqpu.com/gtvkqjgqqm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.andypj.xyz/gtjwdhsrbn.html

[R73] 分割大日志
来源：http://hz.gzhubu.top/gtrujqvuin.html

split -l 1000 big.log part_
来源：http://hz.jiagoushi.top/gthdaexytj.html

[R74] 批量重命名
来源：http://hz.hywenlv.cn/gtfvqrusal.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.haohaochexian.top/gtjogjjynf.html

[R75] 导出环境变量
来源：http://hz.hywenlv.cn/gtrijmmfnv.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhongyouzk.top/gtmdsniycw.html

[R76] 使用临时文件
来源：http://hz.feifeiyinyue.top/gtzvvynjyg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.sysykeji.top/gtyxupvjng.html

[R77] 读取用户输入
来源：http://hz.xuanzx.com/gtguyfhoao.html

read -rp "请输入: " ans
来源：http://hz.hywenlv.cn/gtrmvndlrm.html

[R78] 交互式菜单
来源：http://hz.zhiwuduotai.top/gtujfmbgrw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hnqzz.top/gtvkoltzgi.html

[R79] 解析命令行选项
来源：http://hz.aibaodan.cn/gtivyerbrr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.meibo888.top/gtjucseojh.html

[R80] 查看脚本执行耗时
来源：http://hz.ehwqpu.com/gtqlzaupht.html

time ./run.sh
来源：http://hz.yonumen.top/gtwgmumqzm.html

================================================================================
来源：http://hz.ydzc1.top/gttpcvihkj.html

S. C / C++ 专题
来源：http://hz.sufxvd.cn/gtypzpecbu.html

================================================================================
来源：http://hz.chenlongwang.top/gtjbqrrxpk.html

[S01] C：Hello World
来源：http://hz.tianlin.xyz/gtgqayvznt.html

#include <stdio.h>
来源：http://hz.ywan-chungtsiang.top/gtghdlajub.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yvedp.cn/gtmoidhfev.html

[S02] C：变量与格式化输出
来源：http://hz.zhiwuduotai.top/gtuazbmsyl.html

int a = 10; printf("%d\n", a);
来源：http://hz.xingfuxueyuan.xyz/gtjnrahybi.html

[S03] C：读入整数
来源：http://hz.shanyushiyangtech.top/gthrwkfcgn.html

int x; scanf("%d", &x);
来源：http://hz.guowangkeji.top/gtllfznjcp.html

[S04] C：字符串复制
来源：http://hz.yj20258.top/gthdhpemdh.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.c1oappe.top/gtpznllcem.html

[S05] C：字符串长度
来源：http://hz.shanyushiyangtech.top/gtsyuurqaj.html

strlen(s)
来源：http://hz.mhx1999.top/gtwvmakcex.html

[S06] C：字符串比较
来源：http://hz.fzhhl.top/gtjdpadfpa.html

strcmp(a, b) == 0
来源：http://hz.shanyushiyangkeji.top/gtoonwsamc.html

[S07] C：数组遍历求和
来源：http://hz.fzhhl.top/gtrtopisnn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.shuidangran.top/gtqzrvhxjm.html

[S08] C：动态内存分配与释放
来源：http://hz.havefunace.top/gtvhmrkulm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.chenjidiqi.icu/gtiusglrql.html

[S09] C：结构体定义与初始化
来源：http://hz.birdmap.top/gtpckjjtxc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xylfe.cn/gtytcevusi.html

[S10] C：指针与解引用
来源：http://hz.gaohongyu789.top/gtlzrshioh.html

int *p = &a;  *p = 5;
来源：http://hz.bjfxy.top/gtucuhwgfo.html

[S11] C：逐行读文件
来源：http://hz.mhx1999.top/gtsjdgjpfj.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yj20258888.top/gtepuxhqwg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinghuilouyu.cn/gtihfymoch.html

fclose(f);
来源：http://hz.daxiang520.top/gtyslnfsdb.html

[S12] C：写文件
来源：http://hz.cheryme.top/gtzwzxoabm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jinyuanbaomall.cn/gtysumbbmw.html

[S13] C：宏定义
来源：http://hz.gzhubu.top/gtpfgyiwwe.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yuanzhike.top/gtgbaprpqv.html

[S14] C：枚举
来源：http://hz.yvedp.cn/gttsvysrqe.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.feifeiyinyue.top/gtnixergyr.html

[S15] C：类型转换
来源：http://hz.xuanzx.com/gttjpvdexd.html

(double) a / b
来源：http://hz.andypj.xyz/gtujeykjce.html

[S16] C：位操作置位
来源：http://hz.pycfn.com/gtmyidoufy.html

x |= (1 << 3);
来源：http://hz.svipenyu.cn/gtzzgcsodb.html

[S17] C：安全拼接字符串
来源：http://hz.xziqi.cn/gtalcskqwi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinghuilouyu.cn/gtnfgmyxqg.html

[S18] C：命令行参数
来源：http://hz.316326.xyz/gtcvidljxb.html

int main(int argc, char **argv)
来源：http://hz.chenlongwang.top/gtjgtxqfck.html

[S19] C：快速排序
来源：http://hz.jqgfzy.top/gtlzcdakmg.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shanyushiyangtech.top/gtdnjckgjy.html

[S20] C：二分查找
来源：http://hz.sxryk.cn/gtgrbauiax.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zycfv.cn/gtrhktpuan.html

[S21] C：字符类别判断
来源：http://hz.meibo888.top/gtdskvkqvr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zdqjudy.top/gtpgbsqzjl.html

[S22] C：字符串转数字
来源：http://hz.sweek.top/gtrojiyntr.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.vqdsnc.cn/gtrytitdpj.html

[S23] C：随机数
来源：http://hz.pengpengdd.cyou/gtngiwnqht.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xinyue.icu/gtmrjfiuct.html

[S24] C：获取本地时间
来源：http://hz.316326.xyz/gtsokmanvj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jianghu66.top/gtnmjrrley.html

[S25] C：内存拷贝
来源：http://hz.zhengqikj.top/gtrkqqabjn.html

memcpy(dst, src, n);
来源：http://hz.bjfxy.top/gtfymbscfu.html

[S26] C：内存清零
来源：http://hz.kuanghao11.cn/gtjfiohlgg.html

memset(a, 0, sizeof a);
来源：http://hz.sufxvd.cn/gtbezugtjk.html

[S27] C：定义常量
来源：http://hz.zhengqikj.top/gttytwzjti.html

const double PI = 3.14159;
来源：http://hz.zdqjudy.top/gtamqaaygv.html

[S28] C：静态变量
来源：http://hz.smart0.xyz/gtnuarrbtu.html

static int counter = 0;
来源：http://hz.0kj1m.cn/gtckyrbnit.html

[S29] C：变参函数
来源：http://hz.316326.xyz/gthjkezayg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.vqdsnc.cn/gtnesnextv.html

[S30] C：头文件保护
来源：http://hz.aizwys.cn/gtzzevpwwu.html

#ifndef X_H
来源：http://hz.gotoacloud.top/gtdgzozwrq.html

#define X_H
来源：http://hz.sufxvd.cn/gtgorbyfar.html

#endif
来源：http://hz.pycfn.com/gtoocpgsgr.html

[S31] C++：Hello World
来源：http://hz.hfpthk.cn/gtslhjsajo.html

#include <iostream>
来源：http://hz.sweek.top/gtrpjsaurb.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yvedp.cn/gtejtdzdie.html

[S32] C++：字符串
来源：http://hz.tianlin.xyz/gtlwmhichn.html

std::string s = "hi";  s += "!";
来源：http://hz.cdnleiting.top/gtrdsipquo.html

[S33] C++：vector 增删
来源：http://hz.yonumen.top/gtwmgyuttw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jlsjyb.cn/gtrgzjeqnt.html

[S34] C++：遍历 vector
来源：http://hz.aibaodan.cn/gtulvtubte.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.nanxinkj.top/gtqjwrqvgb.html

[S35] C++：map
来源：http://hz.xuanzx.com/gtwfpbyshb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.redwolf501.top/gtyaucsjms.html

[S36] C++：unordered_map
来源：http://hz.shanyushiyangtech.top/gthrrogrrw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.52xcode.cn/gtfifyinhf.html

[S37] C++：set
来源：http://hz.jqgufenzy.top/gtkmgkcqrz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jyoumei.cn/gtmznfjcrs.html

[S38] C++：排序
来源：http://hz.jianghu66.top/gttlphvepj.html

std::sort(v.begin(), v.end());
来源：http://hz.xylfe.cn/gtqiobmkjh.html

[S39] C++：自定义比较器排序
来源：http://hz.bjfxy.top/gthdqjogvy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhongyouzk.top/gtxpaozsjs.html

[S40] C++：查找元素
来源：http://hz.tianlin.xyz/gtyxhvanrj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xuetiantiany.cn/gteoqcopux.html

[S41] C++：类与构造函数
来源：http://hz.pycfn.com/gttliossrg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.guowangkeji.top/gtzufvxmxy.html

[S42] C++：继承与虚函数
来源：http://hz.jqgufenzy.top/gtgiwwvnqc.html

class B : public Base { public: void f() override {} };
来源：http://hz.yuxming.cn/gtimnvlfoq.html

[S43] C++：智能指针
来源：http://hz.xuetiantiany.cn/gtnbuqxhye.html

auto p = std::make_unique<int>(5);
来源：http://hz.zycfv.cn/gtqbsbwdoz.html

[S44] C++：引用传参
来源：http://hz.hongshengwenyu.top/gtimwxnbff.html

void inc(int &x) { ++x; }
来源：http://hz.havefunace.top/gtvvctbioj.html

[S45] C++：lambda
来源：http://hz.hongshengwenyu.top/gtefmdmutb.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jyoumei.cn/gtmaboheoy.html

[S46] C++：函数模板
来源：http://hz.snrcjt.cn/gtyejmjjnt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ivvv.top/gtmjpxtxju.html


<!-- 参考信息 -->