代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.shanyushiyangkeji.top/gtegqzhtgd.html

[Q75] 日期格式化
来源：http://hz.0kj1m.cn/gtqzyxmpxh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yueranfly.top/gtsrxaygvd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yongpay.top/gtxxangati.html

[Q76] 按天统计
来源：http://hz.pycfn.com/gtaabuyrof.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shanyushiyangkeji.top/gtzvlfxqov.html

[Q77] 时间加减
来源：http://hz.dianchejie.cn/gtwcwdtudk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.tianlin.xyz/gtmozqrxoe.html

[Q78] 当前时间
来源：http://hz.shanyushiyangtech.top/gtsvednxxd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ppjwa.cn/gtagatlery.html

[Q79] 字符串拼接
来源：http://hz.ivvv.top/gtzqqvhasm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hongshengwenyu.top/gthsghiull.html

[Q80] 字符串截取
来源：http://hz.gaohongyu789.top/gttlpgarla.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.aizwys.cn/gtglwazssd.html

[Q81] 字符串替换
来源：http://hz.jyoumei.cn/gthpmufsqg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.bjfxy.top/gtpbhjeydr.html

[Q82] 字符长度与字节长度
来源：http://hz.shangyingyoupin.top/gtjwqwbzhh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.pycfn.com/gtzoetdibi.html

[Q83] 大小写转换
来源：http://hz.yangfankeji.com/gttecnldug.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yonumen.top/gtxljfaapa.html

[Q84] 去除首尾空格
来源：http://hz.cashguo.top/gtxouzubxt.html

SELECT TRIM(name) FROM users;
来源：http://hz.xuanzx.com/gtkicpiscf.html

[Q85] 数值取整
来源：http://hz.zhiwuduotai.top/gtowjmcsjy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ehwqpu.com/gtcrtyjerh.html

[Q86] 读取 JSON 字段
来源：http://hz.jqgufenzy.top/gthhlqkxuv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.aizwys.cn/gtfbjhugbu.html

[Q87] JSON 字段做条件
来源：http://hz.zhaomingkeji.xyz/gtghqtggyz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jlsjyb.cn/gtcovmcrpe.html

[Q88] 行转列（条件聚合）
来源：http://hz.tanke756.top/gtngpmybfm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cdnleiting.top/gtgdhjqvpn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.fzhhl.top/gtoxqvczmj.html

[Q89] 判断表是否存在
来源：http://hz.zhijiandao.cn/gtvknikazt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ydjk.org.cn/gtnukrkviw.html

[Q90] 生成序号列
来源：http://hz.zhaomingkeji.xyz/gtetxiddil.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.tanke756.top/gtpkjvvwwz.html

================================================================================
来源：http://hz.aibaodan.cn/gtvwadhaar.html

R. Bash 专题
来源：http://hz.chenlongwang.top/gtgcuymchj.html

================================================================================
来源：http://hz.52xcode.cn/gtyceeszlp.html

[R01] shebang 与严格模式
来源：http://hz.vqdsnc.cn/gtytgbeaxt.html

#!/usr/bin/env bash
来源：http://hz.haohaochexian.top/gtszpmydan.html

set -euo pipefail
来源：http://hz.jinghuilouyu.cn/gtmehugzbl.html

[R02] 变量赋值与使用
来源：http://hz.yanxiufei.cn/gtwrohencx.html

name="Tom"; echo "$name"
来源：http://hz.jinqigufen.top/gtblgexena.html

[R03] 只读变量
来源：http://hz.jianghu66.top/gttsirojos.html

readonly PI=3.14
来源：http://hz.snrcjt.cn/gtlzfxdnvt.html

[R04] 位置参数
来源：http://hz.meibo888.top/gtkykjqcgb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.nanxinkj.top/gtzsqdntar.html

[R05] 参数默认值
来源：http://hz.zdqjudy.top/gtixecdarr.html

name="${1:-default}"
来源：http://hz.zhaomingkeji.xyz/gtybmpuwvb.html

[R06] 判断命令是否存在
来源：http://hz.guowangkeji.top/gtfcvpvvte.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xuanzx.com/gtjbhymjzf.html

[R07] if 判断文件
来源：http://hz.yuanzhike.top/gttibhsqba.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sufxvd.cn/gtrwwgkzhp.html

[R08] 数值比较
来源：http://hz.cashguo.top/gtgxnkusmu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yuanzhike.top/gtqmabaefn.html

[R09] 字符串比较
来源：http://hz.havefunace.top/gtveyzcdvc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.pycfn.com/gtkunttjvo.html

[R10] 正则匹配
来源：http://hz.cdnleiting.top/gtwfajdlsn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.chenzaomai.com/gtvtddaena.html

[R11] case 多分支
来源：http://hz.quarkkingdee.top/gtksytnmwd.html

case "$1" in
来源：http://hz.shzxlz.cn/gtrbebdhax.html

start) echo "启动" ;;
来源：http://hz.sufxvd.cn/gtsgjokmge.html

stop)  echo "停止" ;;
来源：http://hz.zycfv.cn/gtryfwyiws.html

*)     echo "未知命令" ;;
来源：http://hz.shanyushiyangtech.top/gtwebuknga.html

esac
来源：http://hz.meibo888.top/gtnqkrzhlj.html

[R12] for 遍历文件
来源：http://hz.daxiang520.top/gtcrpyouaq.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jiagoushi.top/gttrgckrfb.html

[R13] for 计数循环
来源：http://hz.yuxming.cn/gtwxaiwtva.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.svipenyu.cn/gthuggjtrx.html

[R14] C 风格 for
来源：http://hz.nanxuanxn.top/gtdoudctdp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hfpthk.cn/gtaxzzuidk.html

[R15] while 逐行读文件
来源：http://hz.xziqi.cn/gtzquivljq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jinyuanbaomall.cn/gtkymrfebl.html

[R16] until 等待条件
来源：http://hz.ywan-chungtsiang.top/gtzbonwvpn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.aizwys.cn/gttshclcgi.html

[R17] 数组定义与取值
来源：http://hz.hywenlv.cn/gtppxbyntu.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yvedp.cn/gtruecevjd.html

[R18] 遍历数组
来源：http://hz.jinqigfzy.top/gteoolwcwq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cashguo.top/gtzqcmjgfi.html

[R19] 数组长度
来源：http://hz.redwolf501.top/gtrppzxlru.html

echo "${#arr[@]}"
来源：http://hz.svipenyu.cn/gtakknisgu.html

[R20] 关联数组（字典）
来源：http://hz.zycfv.cn/gtczxjldya.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.redwolf501.top/gtcfpigoez.html

[R21] 字符串长度
来源：http://hz.hywenlv.cn/gtvmuooqlq.html

echo "${#s}"
来源：http://hz.jqgfzy.top/gteuhsmsip.html

[R22] 截取子串
来源：http://hz.bjfxy.top/gtoywzkggm.html

echo "${s:0:5}"
来源：http://hz.redwolf501.top/gtqbyrwtmc.html

[R23] 字符串替换
来源：http://hz.yuanzhike.top/gtydvxzzfj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shzxlz.cn/gtvctrixaa.html

[R24] 大小写转换
来源：http://hz.c1oappe.top/gtrepddntt.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xinyue.icu/gtwigrasvo.html

[R25] 去后缀 / 去前缀
来源：http://hz.wangshuangyany.cn/gtacaqkumk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ybcxt.top/gttqidoejx.html

[R26] 命令替换
来源：http://hz.bjfxy.top/gtiaduborq.html

now=$(date +%F); echo "$now"
来源：http://hz.nwbrower.top/gtjdfjyzqe.html

[R27] 算术展开
来源：http://hz.redwolf501.top/gtmocrcdof.html

echo $((1 + 2 * 3))
来源：http://hz.fzhhl.top/gtymtbdpvt.html

[R28] 浮点运算
来源：http://hz.xuanzx.com/gtsehfmtmj.html

echo "scale=2; 10/3" | bc
来源：http://hz.gzhubu.top/gtpttpfgqu.html

[R29] 定义函数
来源：http://hz.svipenyu.cn/gtrgezyrkb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sufxvd.cn/gtamikjepe.html

[R30] 函数返回状态码
来源：http://hz.xinyue.icu/gttnuzrjki.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gaohongyu789.top/gtsuryypaz.html

[R31] 局部变量
来源：http://hz.zhongyouzk.top/gteoiwaolj.html

f() { local x=1; echo "$x"; }
来源：http://hz.hongshengwenyu.top/gthdsuxrkm.html

[R32] 参数个数校验
来源：http://hz.mhx1999.top/gtcwbiihkp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.tianlin.xyz/gtlxlpvrez.html

[R33] 捕获错误并提示行号
来源：http://hz.hammf.cn/gtqejjcyva.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.316326.xyz/gtwoyrawcd.html

[R34] 退出时清理
来源：http://hz.hongshengwenyu.top/gtsagoqxnw.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.cashguo.top/gtgtleehyx.html

[R35] 后台执行并等待
来源：http://hz.xziqi.cn/gtspukuwkv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xylfe.cn/gtwrixrqoz.html

[R36] 并发执行多个任务
来源：http://hz.316326.xyz/gthftheajz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.feifeiyinyue.top/gtziqowfrs.html

[R37] 把输出赋给变量
来源：http://hz.shangyingyoupin.top/gtsrrazynj.html

files=$(ls -1)
来源：http://hz.havefunace.top/gtwhfbxflu.html

[R38] 管道串联
来源：http://hz.hysaishi.cn/gtiukmsdiz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.316326.xyz/gtbzvlvtrw.html

[R39] 重定向标准输出与错误
来源：http://hz.chenjidiqi.icu/gtnadxixke.html

cmd > out.log 2>&1
来源：http://hz.c1oappe.top/gtkcauvwhw.html

[R40] 追加写日志
来源：http://hz.yj20258888.top/gtfheadzxu.html

echo "log" >> out.log
来源：http://hz.jianghu66.top/gtvkrqyazj.html

[R41] 丢弃输出
来源：http://hz.jlsjyb.cn/gtbqlvzdpc.html

cmd >/dev/null 2>&1
来源：http://hz.xuetiantiany.cn/gtoagbipwx.html

[R42] 输入重定向
来源：http://hz.fengsongda.top/gtqkvrrlga.html

wc -l < a.txt
来源：http://hz.zhiwuduotai.top/gtnpdhwkhw.html

[R43] 按名字查找文件
来源：http://hz.aizwys.cn/gttdsuwidh.html

find . -name "*.log" -type f
来源：http://hz.yanxiufei.cn/gtcztpwsht.html

[R44] 按修改时间查找
来源：http://hz.sxryk.cn/gtedamkfbq.html

find . -mtime -7 -type f
来源：http://hz.hongshengwenyu.top/gtaripfbvd.html

[R45] 批量删除
来源：http://hz.xziqi.cn/gttjxpgvvr.html

find . -name "*.tmp" -delete
来源：http://hz.jlsjyb.cn/gtoywvepcc.html

[R46] 递归替换文件内容
来源：http://hz.hfpthk.cn/gtyxycdieh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yj20258888.top/gtjlyuhlcm.html

[R47] sed 单行替换
来源：http://hz.bjfxy.top/gtorhphger.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hnxiangtu.top/gtkuzxuped.html

[R48] awk 取指定列
来源：http://hz.xziqi.cn/gtxwqwnjex.html

awk '{print $1, $3}' a.txt
来源：http://hz.daria6918.cn/gtkoseathx.html

[R49] awk 带条件
来源：http://hz.ppjwa.cn/gtgtwtzqoz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.svipenyu.cn/gthcjmdsqk.html

[R50] awk 求和
来源：http://hz.fengsongda.top/gtgpkqclvb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cdnleiting.top/gtwppyftvw.html

[R51] 排序去重取前几
来源：http://hz.shzxlz.cn/gtbpgrauew.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jqgfzy.top/gtswcsxpew.html

[R52] 统计行数
来源：http://hz.xylfe.cn/gtikwjraql.html

wc -l a.txt
来源：http://hz.jinqigfzy.top/gthladbvtr.html

[R53] 查看文件头与实时尾
来源：http://hz.ybcxt.top/gtyrbamovi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.gotoacloud.top/gtzgrodvfa.html

[R54] 比较两个文件
来源：http://hz.redwolf501.top/gtkettwlhw.html

diff a.txt b.txt
来源：http://hz.wangdashe.top/gtadupfirx.html

[R55] 压缩与解压
来源：http://hz.shanyushiyangkeji.top/gtigcxjkvl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jianghu66.top/gtadywfsyz.html

[R56] 远程拷贝
来源：http://hz.hammf.cn/gttwjchhjd.html

scp file user@host:/path/
来源：http://hz.chenlongwang.top/gtgcbwuohy.html

[R57] 远程执行命令
来源：http://hz.hfpthk.cn/gtvytwkrux.html

ssh user@host 'uptime'
来源：http://hz.cucudq.cn/gtkeytzdxc.html

[R58] 下载文件
来源：http://hz.yangfankeji.com/gtsroetmec.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.316326.xyz/gtchnuyikj.html

[R59] 发 POST JSON
来源：http://hz.sxryk.cn/gtvaqhprjv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xinyue.icu/gtyianszev.html

[R60] 只看 HTTP 状态码
来源：http://hz.svipenyu.cn/gtmaipluuh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.fzhhl.top/gtcuyugxmb.html

[R61] 磁盘占用
来源：http://hz.jinqigufen.top/gttzwidfke.html

df -h;  du -sh *
来源：http://hz.gzhubu.top/gtbhkhyiut.html

[R62] 找最占空间的文件
来源：http://hz.birdmap.top/gtrqoqrwop.html

du -ah . | sort -rh | head -10
来源：http://hz.daria6918.cn/gtungomlfi.html

[R63] 内存与进程
来源：http://hz.yj20258888.top/gtpifjcstj.html

free -h;  ps aux | grep nginx
来源：http://hz.zhiwuduotai.top/gtcwtwetbk.html

[R64] 结束进程
来源：http://hz.jinqigufen.top/gtnfakunyd.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cqqwz.cn/gtxllfeuja.html

[R65] 查看端口占用
来源：http://hz.vqdsnc.cn/gthmczdfgg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.mhx1999.top/gtaoslvxhw.html

[R66] 定时任务
来源：http://hz.tianlin.xyz/gtqtitevqh.html

crontab -e;  crontab -l
来源：http://hz.kuanghao11.cn/gthqoysbsi.html

[R67] 生成随机十六进制串
来源：http://hz.yj20258888.top/gtspjyrtdm.html

openssl rand -hex 16
来源：http://hz.yueranfly.top/gtxjuyxthq.html

[R68] 计算文件校验值
来源：http://hz.shangyingyoupin.top/gtfquamlrw.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xingfuxueyuan.xyz/gtsbsikxgf.html

[R69] 生成随机密码
来源：http://hz.hongshengwenyu.top/gtynzokuda.html

head -c 16 /dev/urandom | base64
来源：http://hz.hammf.cn/gtuusxippt.html

[R70] 时间戳与互转
来源：http://hz.vqdsnc.cn/gtohstwqfg.html

date +%s;  date -d @1700000000
来源：http://hz.ybcxt.top/gtghmpeecx.html

[R71] 日期格式化
来源：http://hz.yongpay.top/gtkxwihyuu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.havefunace.top/gttpnglzhs.html

[R72] 等待端口就绪
来源：http://hz.jqgfzy.top/gtstisjjac.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yuxming.cn/gtsmlqpdct.html

[R73] 分割大日志
来源：http://hz.xziqi.cn/gtynhuxlpl.html

split -l 1000 big.log part_
来源：http://hz.hongshengwenyu.top/gtjbarbkla.html

[R74] 批量重命名
来源：http://hz.ivvv.top/gtglfjyagu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zycfv.cn/gtkjzdhgbn.html

[R75] 导出环境变量
来源：http://hz.52xcode.cn/gtyswdwlob.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yuanzhike.top/gtntadjgvp.html

[R76] 使用临时文件
来源：http://hz.xziqi.cn/gtznfidchf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yuxming.cn/gtjzvryulm.html

[R77] 读取用户输入
来源：http://hz.zdqjudy.top/gtnksevinu.html

read -rp "请输入: " ans
来源：http://hz.havefunace.top/gtufyrtziu.html

[R78] 交互式菜单
来源：http://hz.cqqwz.cn/gtzygfshmu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zdqjudy.top/gtwrmnekhj.html

[R79] 解析命令行选项
来源：http://hz.nanxuanxn.top/gtnbypianz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.aizwys.cn/gthnztmsaa.html

[R80] 查看脚本执行耗时
来源：http://hz.cdnleiting.top/gtilxulkwi.html

time ./run.sh
来源：http://hz.jqgfzy.top/gtzpsqfsgq.html

================================================================================
来源：http://hz.yanxiufei.cn/gtqqvambbc.html

S. C / C++ 专题
来源：http://hz.havefunace.top/gtnfcdllcz.html

================================================================================
来源：http://hz.shuidangran.top/gtqxlzbjew.html

[S01] C：Hello World
来源：http://hz.zhengqikj.top/gtgyukvouo.html

#include <stdio.h>
来源：http://hz.zhiwuduotai.top/gtioeipiqm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.vqdsnc.cn/gtcbzsbhwj.html

[S02] C：变量与格式化输出
来源：http://hz.gotoacloud.top/gtmceadofx.html

int a = 10; printf("%d\n", a);
来源：http://hz.ydjk.org.cn/gtwprtuzyl.html

[S03] C：读入整数
来源：http://hz.sysykeji.top/gtptinpnvy.html

int x; scanf("%d", &x);
来源：http://hz.xuetiantiany.cn/gtxowjxyyh.html

[S04] C：字符串复制
来源：http://hz.sxryk.cn/gtwgchvrxx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jlsjyb.cn/gtleyydlpr.html

[S05] C：字符串长度
来源：http://hz.birdmap.top/gtmxadkfes.html

strlen(s)
来源：http://hz.jyoumei.cn/gtuwjhuexl.html

[S06] C：字符串比较
来源：http://hz.birdmap.top/gtqmuqsfmz.html

strcmp(a, b) == 0
来源：http://hz.gaohongyu789.top/gtcfxaavxe.html

[S07] C：数组遍历求和
来源：http://hz.xingfuxueyuan.xyz/gtzgrmcrno.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.tianlin.xyz/gtxxdwqubs.html

[S08] C：动态内存分配与释放
来源：http://hz.jqgfzy.top/gtcvodybap.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.daxiang520.top/gtsjmywlqf.html

[S09] C：结构体定义与初始化
来源：http://hz.dianchejie.cn/gtwcklzwwv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ywan-chungtsiang.top/gtdsbojrsh.html

[S10] C：指针与解引用
来源：http://hz.bjfxy.top/gtmvfsngxo.html

int *p = &a;  *p = 5;
来源：http://hz.sxryk.cn/gtsxlcnvoq.html

[S11] C：逐行读文件
来源：http://hz.xziqi.cn/gtaolsfpys.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.dianchejie.cn/gtdzkfruld.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hfpthk.cn/gtptadqpnq.html

fclose(f);
来源：http://hz.daria6918.cn/gtfrfyoeyd.html

[S12] C：写文件
来源：http://hz.jqgfzy.top/gtxcxzsqod.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.52xcode.cn/gtaifguvww.html

[S13] C：宏定义
来源：http://hz.shuidangran.top/gtmushokri.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.andypj.xyz/gtbdkgimym.html

[S14] C：枚举
来源：http://hz.hfpthk.cn/gtuqycojmk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jinqigfzy.top/gtclxpbezd.html

[S15] C：类型转换
来源：http://hz.jinqigufen.top/gtzecyccyp.html

(double) a / b
来源：http://hz.chenjidiqi.icu/gteozrvnlu.html

[S16] C：位操作置位
来源：http://hz.yonumen.top/gtimixtrbr.html

x |= (1 << 3);
来源：http://hz.ehwqpu.com/gtfowduvjf.html

[S17] C：安全拼接字符串
来源：http://hz.hywenlv.cn/gtqritqpjb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ppjwa.cn/gtuocimstx.html

[S18] C：命令行参数
来源：http://hz.chenzaomai.com/gtkmesuuna.html

int main(int argc, char **argv)
来源：http://hz.cashguo.top/gtdgmdsqsu.html

[S19] C：快速排序
来源：http://hz.jinghuilouyu.cn/gttddnbjuo.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cashguo.top/gtheqmhyhk.html

[S20] C：二分查找
来源：http://hz.xuetiantiany.cn/gtpjrnqwrh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.316326.xyz/gtnrzkiecm.html

[S21] C：字符类别判断
来源：http://hz.nanxinkj.top/gtjyhlrxab.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.nanxinkj.top/gtwujltrbb.html

[S22] C：字符串转数字
来源：http://hz.ydzc1.top/gtelwvzvht.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.chenlongwang.top/gtzwspznhl.html

[S23] C：随机数
来源：http://hz.svipenyu.cn/gtjbupvbxz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.dianchejie.cn/gtkpddixuj.html

[S24] C：获取本地时间
来源：http://hz.feifeiyinyue.top/gthymcyheh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.c1oappe.top/gtokyzmjwl.html

[S25] C：内存拷贝
来源：http://hz.redwolf501.top/gtqmphnlif.html

memcpy(dst, src, n);
来源：http://hz.yj202588.top/gtvwatqfrz.html

[S26] C：内存清零
来源：http://hz.wangdashe.top/gtftjbdcis.html

memset(a, 0, sizeof a);
来源：http://hz.fzhhl.top/gtcishmudp.html

[S27] C：定义常量
来源：http://hz.snrcjt.cn/gtyrdsoqte.html

const double PI = 3.14159;
来源：http://hz.yuanzhike.top/gtbkpkiwlv.html

[S28] C：静态变量
来源：http://hz.yj20258888.top/gtikrpetcz.html

static int counter = 0;
来源：http://hz.pengpengdd.cyou/gtkjcunbkq.html

[S29] C：变参函数
来源：http://hz.yuanzhike.top/gtlojlzipn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jqgfzy.top/gtjfbzltqa.html

[S30] C：头文件保护
来源：http://hz.jqgfzy.top/gteeoxmfte.html

#ifndef X_H
来源：http://hz.gogol.net.cn/gtpqaszude.html

#define X_H
来源：http://hz.zhiwuduotai.top/gtnrwtsbgg.html

#endif
来源：http://hz.meibo888.top/gtaxfhyltp.html

[S31] C++：Hello World
来源：http://hz.jlsjyb.cn/gtubyftqvb.html

#include <iostream>
来源：http://hz.dashuyun.cn/gtucjlgfuf.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.haohaochexian.top/gtqjgdhsgh.html

[S32] C++：字符串
来源：http://hz.shanyushiyangkeji.top/gtvvjrurpw.html

std::string s = "hi";  s += "!";
来源：http://hz.yvedp.cn/gtiwvegewq.html

[S33] C++：vector 增删
来源：http://hz.gogol.net.cn/gtxlzgmgjm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.gogol.net.cn/gtwesxlwpn.html

[S34] C++：遍历 vector
来源：http://hz.jinyuanbaomall.cn/gtoemfatng.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xziqi.cn/gtnvgyowpu.html

[S35] C++：map
来源：http://hz.52xcode.cn/gtmonmvrww.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jqgufenzy.top/gtyilhscyt.html

[S36] C++：unordered_map
来源：http://hz.haohaochexian.top/gtbddfrzlr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cucudq.cn/gtebiydtxg.html

[S37] C++：set
来源：http://hz.smart0.xyz/gtmgxjaszz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yueranfly.top/gtzmerzadq.html

[S38] C++：排序
来源：http://hz.cheryme.top/gtvvflhhur.html

std::sort(v.begin(), v.end());
来源：http://hz.nanxuanxn.top/gtxdnsqqsn.html

[S39] C++：自定义比较器排序
来源：http://hz.fengsongda.top/gtikpuosvh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ehwqpu.com/gtpocjkpbk.html

[S40] C++：查找元素
来源：http://hz.birdmap.top/gtoysbbwnq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.sweek.top/gtyfnxkcnc.html

[S41] C++：类与构造函数
来源：http://hz.dianchejie.cn/gtliqaponc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.gogol.net.cn/gtojukqmrq.html

[S42] C++：继承与虚函数
来源：http://hz.dianchejie.cn/gtfjiykzih.html

class B : public Base { public: void f() override {} };
来源：http://hz.jqgfzy.top/gtsmvdqcov.html

[S43] C++：智能指针
来源：http://hz.chenjidiqi.icu/gttciyfovq.html

auto p = std::make_unique<int>(5);
来源：http://hz.cashguo.top/gtuqwcfbee.html

[S44] C++：引用传参
来源：http://hz.cashguo.top/gtlkjfmodc.html

void inc(int &x) { ++x; }
来源：http://hz.yangfankeji.com/gtpuioepta.html


<!-- 参考信息 -->