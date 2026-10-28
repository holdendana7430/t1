代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xingfuxueyuan.xyz/gtgbfcudpl.html

[Q75] 日期格式化
来源：http://hz.aizwys.cn/gtppztnulm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ydzc1.top/gtxirmszrj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhiwuduotai.top/gthjycacan.html

[Q76] 按天统计
来源：http://hz.jinqigfzy.top/gtgykjvsbq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhiwuduotai.top/gtifyecqvu.html

[Q77] 时间加减
来源：http://hz.shanyushiyangkeji.top/gtcggjatfp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yuxming.cn/gtnzlbuazy.html

[Q78] 当前时间
来源：http://hz.0kj1m.cn/gtfbdhykit.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cqqwz.cn/gtunkvjgzq.html

[Q79] 字符串拼接
来源：http://hz.xylfe.cn/gtvnllafie.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.birdmap.top/gtavvkcqkz.html

[Q80] 字符串截取
来源：http://hz.xylfe.cn/gtnxxcmzlt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zdqjudy.top/gtmqprlthi.html

[Q81] 字符串替换
来源：http://hz.nwbrower.top/gtdgoxurbn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jinyuanbaomall.cn/gtxvlsmfwl.html

[Q82] 字符长度与字节长度
来源：http://hz.ydzc1.top/gtnlscreum.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ppjwa.cn/gtqmxffzxr.html

[Q83] 大小写转换
来源：http://hz.cashguo.top/gtukspvhuf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.9152youxi.cn/gtfxrtsqwa.html

[Q84] 去除首尾空格
来源：http://hz.yangfankeji.com/gtxihovlis.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtilnndgrq.html

[Q85] 数值取整
来源：http://hz.gzhubu.top/gtzxnifaka.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhoulong.xyz/gtqgoofemd.html

[Q86] 读取 JSON 字段
来源：http://hz.cucudq.cn/gtawvsflwe.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.wangshuangyany.cn/gtrnnukzuv.html

[Q87] JSON 字段做条件
来源：http://hz.fengsongda.top/gtxibnhxvi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.fzhhl.top/gtlhviuilg.html

[Q88] 行转列（条件聚合）
来源：http://hz.shangyingyoupin.top/gtdmukeyoo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.shanyushiyangtech.top/gtxggmcqfw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.mhx1999.top/gtxykvxjcy.html

[Q89] 判断表是否存在
来源：http://hz.yj202588.top/gtrnedktfx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.sysykeji.top/gtsdpfagrp.html

[Q90] 生成序号列
来源：http://hz.jyoumei.cn/gtqknhcaqu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhengqikj.top/gtcurmdppv.html

================================================================================
来源：http://hz.yj20258888.top/gtdnxunsfu.html

R. Bash 专题
来源：http://hz.jlsjyb.cn/gtaromrbie.html

================================================================================
来源：http://hz.xuanzx.com/gtnwekqwrq.html

[R01] shebang 与严格模式
来源：http://hz.sufxvd.cn/gtbzpenzfx.html

#!/usr/bin/env bash
来源：http://hz.fengsongda.top/gtxwykwzyk.html

set -euo pipefail
来源：http://hz.jinghuilouyu.cn/gthywzryit.html

[R02] 变量赋值与使用
来源：http://hz.yj202588.top/gtteiiywai.html

name="Tom"; echo "$name"
来源：http://hz.xinyue.icu/gtatokmhkh.html

[R03] 只读变量
来源：http://hz.jiagoushi.top/gtighvbvoe.html

readonly PI=3.14
来源：http://hz.jyoumei.cn/gtgnnghquz.html

[R04] 位置参数
来源：http://hz.wangshuangyany.cn/gtspgqootz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jiagoushi.top/gtndbnuuir.html

[R05] 参数默认值
来源：http://hz.hnqzz.top/gtdeqkosao.html

name="${1:-default}"
来源：http://hz.shangyingyoupin.top/gtmuodvvuw.html

[R06] 判断命令是否存在
来源：http://hz.zhoulong.xyz/gtgpmjifdh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhengqikj.top/gtneokwfre.html

[R07] if 判断文件
来源：http://hz.zhaomingkeji.xyz/gtqwumszpt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xingfuxueyuan.xyz/gtajitgmdg.html

[R08] 数值比较
来源：http://hz.cdnleiting.top/gtjfcgflbg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ehwqpu.com/gttllqogwn.html

[R09] 字符串比较
来源：http://hz.kuanghao11.cn/gtudwcqvix.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.fengsongda.top/gtynfbvrye.html

[R10] 正则匹配
来源：http://hz.sysykeji.top/gtxhsiegcc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.mhx1999.top/gtfkdhtrrh.html

[R11] case 多分支
来源：http://hz.gaohongyu789.top/gthyyryycd.html

case "$1" in
来源：http://hz.ydzc1.top/gtwucqqfbe.html

start) echo "启动" ;;
来源：http://hz.pycfn.com/gtjwptgwwg.html

stop)  echo "停止" ;;
来源：http://hz.svipenyu.cn/gtfnbbvjbm.html

*)     echo "未知命令" ;;
来源：http://hz.jianghu66.top/gtymnemlme.html

esac
来源：http://hz.ybcxt.top/gtzljiubvs.html

[R12] for 遍历文件
来源：http://hz.jqgufenzy.top/gtkqfdtyqc.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhiwuduotai.top/gtuuzbepai.html

[R13] for 计数循环
来源：http://hz.jyoumei.cn/gtaicbteyi.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yuanzhike.top/gtzhvxccaj.html

[R14] C 风格 for
来源：http://hz.cheryme.top/gtiblkrorq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.svipenyu.cn/gtkhlnupju.html

[R15] while 逐行读文件
来源：http://hz.ehwqpu.com/gtmyeoywmg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.gzhubu.top/gtechoydqg.html

[R16] until 等待条件
来源：http://hz.tian-w.cn/gttdtnbmuz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.tian-w.cn/gtcxjhwjqx.html

[R17] 数组定义与取值
来源：http://hz.yueranfly.top/gtzeshaort.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jqgfzy.top/gtqqumdwdy.html

[R18] 遍历数组
来源：http://hz.jinghuilouyu.cn/gtewzyxywy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhaomingkeji.xyz/gtdvpduwet.html

[R19] 数组长度
来源：http://hz.xinyue.icu/gtpfkrrlbs.html

echo "${#arr[@]}"
来源：http://hz.redwolf501.top/gtpynmiutv.html

[R20] 关联数组（字典）
来源：http://hz.daria6918.cn/gtnfgpvehh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xuetiantiany.cn/gtnqsmnavc.html

[R21] 字符串长度
来源：http://hz.jinqigfzy.top/gtonrdrrud.html

echo "${#s}"
来源：http://hz.ydjk.org.cn/gtcngrungw.html

[R22] 截取子串
来源：http://hz.hywenlv.cn/gtnfynotdw.html

echo "${s:0:5}"
来源：http://hz.zhaomingkeji.xyz/gtryirlhkq.html

[R23] 字符串替换
来源：http://hz.wangshuangyany.cn/gtlxudxiag.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhongyouzk.top/gtponopedd.html

[R24] 大小写转换
来源：http://hz.cashguo.top/gtzcjypymm.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.gzhubu.top/gtzldmitrw.html

[R25] 去后缀 / 去前缀
来源：http://hz.nwbrower.top/gtkfevlmtw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ppjwa.cn/gtyehwnedv.html

[R26] 命令替换
来源：http://hz.dashuyun.cn/gtvwnzbmys.html

now=$(date +%F); echo "$now"
来源：http://hz.sweek.top/gtdxnnyvhh.html

[R27] 算术展开
来源：http://hz.zhengqikj.top/gtcxhmrbyo.html

echo $((1 + 2 * 3))
来源：http://hz.zycfv.cn/gtvvpedbwz.html

[R28] 浮点运算
来源：http://hz.dianchejie.cn/gtsbbdatcb.html

echo "scale=2; 10/3" | bc
来源：http://hz.yj20258888.top/gtgoocwatc.html

[R29] 定义函数
来源：http://hz.daria6918.cn/gtohbgmhyq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jinghuilouyu.cn/gtoprtmfmd.html

[R30] 函数返回状态码
来源：http://hz.sxryk.cn/gthwesifpx.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yj202588.top/gtfpuaszgy.html

[R31] 局部变量
来源：http://hz.yvedp.cn/gtcsqfqymg.html

f() { local x=1; echo "$x"; }
来源：http://hz.yangfankeji.com/gttcviwfnz.html

[R32] 参数个数校验
来源：http://hz.xinyue.icu/gtrxetnjqu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ydjk.org.cn/gtqtxuesgu.html

[R33] 捕获错误并提示行号
来源：http://hz.cdnleiting.top/gtipjhcuzu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.dashuyun.cn/gtvrbkpaev.html

[R34] 退出时清理
来源：http://hz.dashuyun.cn/gtzqlkzdwa.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zycfv.cn/gtkbqpvubs.html

[R35] 后台执行并等待
来源：http://hz.nanxuanxn.top/gtvlxfukyq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.aizwys.cn/gtlxdjvfpl.html

[R36] 并发执行多个任务
来源：http://hz.hywenlv.cn/gtsikgjhsc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hnqzz.top/gtlkzeyiiy.html

[R37] 把输出赋给变量
来源：http://hz.cqqwz.cn/gtwoakhxwp.html

files=$(ls -1)
来源：http://hz.sweek.top/gtqgzgbtmp.html

[R38] 管道串联
来源：http://hz.gzhubu.top/gttntwflkb.html

cat a.txt | grep -i error | wc -l
来源：http://hz.52xcode.cn/gtxcxquvsj.html

[R39] 重定向标准输出与错误
来源：http://hz.cashguo.top/gtkwwyafww.html

cmd > out.log 2>&1
来源：http://hz.316326.xyz/gtaqrgawwe.html

[R40] 追加写日志
来源：http://hz.haohaochexian.top/gtgeqqzrkh.html

echo "log" >> out.log
来源：http://hz.hfpthk.cn/gtxzgvxgje.html

[R41] 丢弃输出
来源：http://hz.aizwys.cn/gtytoxcgoo.html

cmd >/dev/null 2>&1
来源：http://hz.chenjidiqi.icu/gtxycjetdk.html

[R42] 输入重定向
来源：http://hz.yj202588.top/gtgtymqrmx.html

wc -l < a.txt
来源：http://hz.9152youxi.cn/gtixkfclep.html

[R43] 按名字查找文件
来源：http://hz.jinyuanbaomall.cn/gtsqzkdush.html

find . -name "*.log" -type f
来源：http://hz.sufxvd.cn/gtiawavlxd.html

[R44] 按修改时间查找
来源：http://hz.yvedp.cn/gtytcsobjy.html

find . -mtime -7 -type f
来源：http://hz.sufxvd.cn/gtpznywbtk.html

[R45] 批量删除
来源：http://hz.aizwys.cn/gtzwbhdzis.html

find . -name "*.tmp" -delete
来源：http://hz.chenlongwang.top/gtztkilcpy.html

[R46] 递归替换文件内容
来源：http://hz.meibo888.top/gtnwmscyxg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ywan-chungtsiang.top/gtutqiuavv.html

[R47] sed 单行替换
来源：http://hz.shanyushiyangkeji.top/gtfwpzzqtc.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.quarkkingdee.top/gtavjobild.html

[R48] awk 取指定列
来源：http://hz.xuanzx.com/gtwvcnfaap.html

awk '{print $1, $3}' a.txt
来源：http://hz.pengpengdd.cyou/gtwhpbgado.html

[R49] awk 带条件
来源：http://hz.ydzc1.top/gtobnxgjdi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yongpay.top/gtouogdkuq.html

[R50] awk 求和
来源：http://hz.shzxlz.cn/gtujveucrm.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.havefunace.top/gtbjdimnyq.html

[R51] 排序去重取前几
来源：http://hz.wangshuangyany.cn/gtnyueanhc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.wangshuangyany.cn/gtloykmkgd.html

[R52] 统计行数
来源：http://hz.gzhubu.top/gtqzgalclp.html

wc -l a.txt
来源：http://hz.sxryk.cn/gtqwrbtggz.html

[R53] 查看文件头与实时尾
来源：http://hz.haohaochexian.top/gtrizkmheg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jqgfzy.top/gtwjmubhfd.html

[R54] 比较两个文件
来源：http://hz.jinqigfzy.top/gtjtzvvhmr.html

diff a.txt b.txt
来源：http://hz.cqqwz.cn/gtdtpxztij.html

[R55] 压缩与解压
来源：http://hz.yongpay.top/gthzyaujek.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xziqi.cn/gttrtwfptx.html

[R56] 远程拷贝
来源：http://hz.xuetiantiany.cn/gttuzwtwvf.html

scp file user@host:/path/
来源：http://hz.ybcxt.top/gtkhyzhveb.html

[R57] 远程执行命令
来源：http://hz.aizwys.cn/gtchsofwcp.html

ssh user@host 'uptime'
来源：http://hz.ybcxt.top/gtdgdjpvzo.html

[R58] 下载文件
来源：http://hz.shanyushiyangkeji.top/gtdaaixdlo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jyoumei.cn/gtscbplfpy.html

[R59] 发 POST JSON
来源：http://hz.xinyue.icu/gteeupsglc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhongyouzk.top/gtvtjowkah.html

[R60] 只看 HTTP 状态码
来源：http://hz.guannengcc.top/gtbawcopxt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.haohaochexian.top/gtgzonqzma.html

[R61] 磁盘占用
来源：http://hz.havefunace.top/gtwkireivc.html

df -h;  du -sh *
来源：http://hz.ppjwa.cn/gtngmkjkca.html

[R62] 找最占空间的文件
来源：http://hz.aibaodan.cn/gttdppustv.html

du -ah . | sort -rh | head -10
来源：http://hz.nanxuanxn.top/gthetcmlky.html

[R63] 内存与进程
来源：http://hz.yonumen.top/gtthcqnafg.html

free -h;  ps aux | grep nginx
来源：http://hz.snrcjt.cn/gthkeuzqjh.html

[R64] 结束进程
来源：http://hz.shanyushiyangkeji.top/gtkcdnlduw.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jlsjyb.cn/gtvmphxqix.html

[R65] 查看端口占用
来源：http://hz.xylfe.cn/gtippzarsh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.svipenyu.cn/gthnkyouqa.html

[R66] 定时任务
来源：http://hz.yueranfly.top/gtewyjcrag.html

crontab -e;  crontab -l
来源：http://hz.mhx1999.top/gtosiesaij.html

[R67] 生成随机十六进制串
来源：http://hz.mhx1999.top/gtrzlkjeoc.html

openssl rand -hex 16
来源：http://hz.yj20258.top/gtcnzwqnvy.html

[R68] 计算文件校验值
来源：http://hz.hammf.cn/gtbuphmasy.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.daxiang520.top/gttkrmpidb.html

[R69] 生成随机密码
来源：http://hz.sweek.top/gtusavfrwx.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhaomingkeji.xyz/gtsxxjperb.html

[R70] 时间戳与互转
来源：http://hz.yj202588.top/gtkmnhypnm.html

date +%s;  date -d @1700000000
来源：http://hz.daria6918.cn/gtehqxshhg.html

[R71] 日期格式化
来源：http://hz.jqgfzy.top/gtdougsjet.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yangfankeji.com/gtnfnfjcrl.html

[R72] 等待端口就绪
来源：http://hz.jlsjyb.cn/gtfveubxmv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ivvv.top/gtmvkrafkk.html

[R73] 分割大日志
来源：http://hz.yj20258888.top/gtyvgblytc.html

split -l 1000 big.log part_
来源：http://hz.yueranfly.top/gtpnuqjfkp.html

[R74] 批量重命名
来源：http://hz.gotoacloud.top/gtnfeokyjm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cqqwz.cn/gtugfbjwxo.html

[R75] 导出环境变量
来源：http://hz.gaohongyu789.top/gtvgsiquck.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.quarkkingdee.top/gtvuibvpuo.html

[R76] 使用临时文件
来源：http://hz.birdmap.top/gtnsjvqwkw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnxiangtu.top/gthxktndqm.html

[R77] 读取用户输入
来源：http://hz.gogol.net.cn/gtpyhqyrli.html

read -rp "请输入: " ans
来源：http://hz.tanke756.top/gtzbrljydt.html

[R78] 交互式菜单
来源：http://hz.ivvv.top/gtvckoxzas.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.tanke756.top/gtcqzvuzzs.html

[R79] 解析命令行选项
来源：http://hz.redwolf501.top/gtgbenzpgo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhengqikj.top/gtvspnibma.html

[R80] 查看脚本执行耗时
来源：http://hz.sweek.top/gtqauqqdii.html

time ./run.sh
来源：http://hz.yvedp.cn/gtbnycceeo.html

================================================================================
来源：http://hz.guannengcc.top/gtndwaonbv.html

S. C / C++ 专题
来源：http://hz.chenzaomai.com/gtpyshwzyi.html

================================================================================
来源：http://hz.zhongyouzk.top/gtgunpfvxo.html

[S01] C：Hello World
来源：http://hz.yueranfly.top/gthvhpcbne.html

#include <stdio.h>
来源：http://hz.xingfuxueyuan.xyz/gtufuierim.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.iojbl.cn/gtlwguungs.html

[S02] C：变量与格式化输出
来源：http://hz.hywenlv.cn/gtbmssortz.html

int a = 10; printf("%d\n", a);
来源：http://hz.hammf.cn/gtajsbqicg.html

[S03] C：读入整数
来源：http://hz.guannengcc.top/gtwsdagsaq.html

int x; scanf("%d", &x);
来源：http://hz.nanxinkj.top/gtazjwodvu.html

[S04] C：字符串复制
来源：http://hz.ybcxt.top/gthuablgrr.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.tianlin.xyz/gtffoohins.html

[S05] C：字符串长度
来源：http://hz.mhx1999.top/gtiaironxi.html

strlen(s)
来源：http://hz.ybcxt.top/gtsgqdgkgt.html

[S06] C：字符串比较
来源：http://hz.cheryme.top/gtuttmkzau.html

strcmp(a, b) == 0
来源：http://hz.haohaochexian.top/gtzlfisxpa.html

[S07] C：数组遍历求和
来源：http://hz.snrcjt.cn/gtefwogulq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.snrcjt.cn/gtwgggtjel.html

[S08] C：动态内存分配与释放
来源：http://hz.cdnleiting.top/gtufkwkbrh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hnxiangtu.top/gthdtzhjta.html

[S09] C：结构体定义与初始化
来源：http://hz.zycfv.cn/gthcodcvyn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yj20258888.top/gtygceyraq.html

[S10] C：指针与解引用
来源：http://hz.fzhhl.top/gtnryjiaao.html

int *p = &a;  *p = 5;
来源：http://hz.zhoulong.xyz/gtpwhzdimj.html

[S11] C：逐行读文件
来源：http://hz.yangfankeji.com/gteanodpgu.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jiagoushi.top/gtdkkgabgt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.cucudq.cn/gthhyuhqxe.html

fclose(f);
来源：http://hz.ybcxt.top/gtrdvnddki.html

[S12] C：写文件
来源：http://hz.shzxlz.cn/gtubiiydxe.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.wangdashe.top/gtacjatrka.html

[S13] C：宏定义
来源：http://hz.jqgufenzy.top/gtjmuqrjih.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.tianlin.xyz/gtrarwwzcd.html

[S14] C：枚举
来源：http://hz.shzxlz.cn/gtpyqqiiwg.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.havefunace.top/gthhnyulim.html

[S15] C：类型转换
来源：http://hz.zhengqikj.top/gtgfrqlbzt.html

(double) a / b
来源：http://hz.jinyuanbaomall.cn/gtkbnsxlck.html

[S16] C：位操作置位
来源：http://hz.hfpthk.cn/gtuaznplqh.html

x |= (1 << 3);
来源：http://hz.jinghuilouyu.cn/gtbswrmktv.html

[S17] C：安全拼接字符串
来源：http://hz.shzxlz.cn/gtnkbeeqhj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhengqikj.top/gtolbzxtqo.html

[S18] C：命令行参数
来源：http://hz.jiagoushi.top/gtohoshtnf.html

int main(int argc, char **argv)
来源：http://hz.zhongyouzk.top/gtbevgoiej.html

[S19] C：快速排序
来源：http://hz.aibaodan.cn/gtdgjoaskr.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.0kj1m.cn/gtfqnjdxer.html

[S20] C：二分查找
来源：http://hz.zhengqikj.top/gtpkufjxce.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cucudq.cn/gtmvomejos.html

[S21] C：字符类别判断
来源：http://hz.sufxvd.cn/gtjxrlyvng.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.feifeiyinyue.top/gtdhemwwrt.html

[S22] C：字符串转数字
来源：http://hz.zhoulong.xyz/gtorsglqbe.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.aizwys.cn/gtehkftzsa.html

[S23] C：随机数
来源：http://hz.yanxiufei.cn/gtazqyenqn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.fzhhl.top/gtvdeuuzib.html

[S24] C：获取本地时间
来源：http://hz.c1oappe.top/gtgmzdroou.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.nwbrower.top/gtykdbsmsi.html

[S25] C：内存拷贝
来源：http://hz.jyoumei.cn/gtodoexjow.html

memcpy(dst, src, n);
来源：http://hz.ppjwa.cn/gtyfijkqka.html

[S26] C：内存清零
来源：http://hz.bjfxy.top/gtezoabwla.html

memset(a, 0, sizeof a);
来源：http://hz.meibo888.top/gtcgkvwjma.html

[S27] C：定义常量
来源：http://hz.meibo888.top/gtipaozugk.html

const double PI = 3.14159;
来源：http://hz.jinqigufen.top/gtxqhetwpv.html

[S28] C：静态变量
来源：http://hz.gogol.net.cn/gtoiccrawc.html

static int counter = 0;
来源：http://hz.aizwys.cn/gtkmcysxcx.html

[S29] C：变参函数
来源：http://hz.xylfe.cn/gttjzhozuq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zycfv.cn/gtrxtcqcgs.html

[S30] C：头文件保护
来源：http://hz.fengsongda.top/gtgqipgqdn.html

#ifndef X_H
来源：http://hz.jianghu66.top/gtdkwspeju.html

#define X_H
来源：http://hz.wangshuangyany.cn/gtvkzbewwy.html

#endif
来源：http://hz.haohaochexian.top/gtkfpmpuyp.html

[S31] C++：Hello World
来源：http://hz.jqgfzy.top/gtawcrdmah.html

#include <iostream>
来源：http://hz.yangfankeji.com/gtgdswmsgh.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yonumen.top/gtfvlfusro.html

[S32] C++：字符串
来源：http://hz.sufxvd.cn/gtbtuwcmoj.html

std::string s = "hi";  s += "!";
来源：http://hz.jlsjyb.cn/gtgovpcktu.html

[S33] C++：vector 增删
来源：http://hz.jinghuilouyu.cn/gtmvbymuts.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.nanxuanxn.top/gtqbvovzkc.html

[S34] C++：遍历 vector
来源：http://hz.vqdsnc.cn/gtwlttcryj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ivvv.top/gtttwccnwx.html

[S35] C++：map
来源：http://hz.shanyushiyangkeji.top/gtchqeogkf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sysykeji.top/gtbvzdkfxn.html

[S36] C++：unordered_map
来源：http://hz.daxiang520.top/gtxcqdzxmf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhixingplan.top/gtmgaywjzg.html

[S37] C++：set
来源：http://hz.nanxinkj.top/gtysarzcxz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.sweek.top/gtfwbxbgrr.html

[S38] C++：排序
来源：http://hz.fengsongda.top/gtmeyrthcj.html

std::sort(v.begin(), v.end());
来源：http://hz.zhaomingkeji.xyz/gtzdjtfmni.html

[S39] C++：自定义比较器排序
来源：http://hz.zhiwuduotai.top/gtgfxluzbh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.nanxinkj.top/gteqxoyddq.html

[S40] C++：查找元素
来源：http://hz.yj20258888.top/gtcudtdfwa.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gotoacloud.top/gtajrxlemh.html

[S41] C++：类与构造函数
来源：http://hz.ywan-chungtsiang.top/gtibouhomb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yanxiufei.cn/gtvzrarhww.html

[S42] C++：继承与虚函数
来源：http://hz.jianghu66.top/gtfskksjxo.html

class B : public Base { public: void f() override {} };
来源：http://hz.ydjk.org.cn/gthpkkoftj.html

[S43] C++：智能指针
来源：http://hz.jlsjyb.cn/gtphqjrqmm.html

auto p = std::make_unique<int>(5);
来源：http://hz.yuanzhike.top/gtyypampjm.html

[S44] C++：引用传参
来源：http://hz.tian-w.cn/gtmtnievns.html

void inc(int &x) { ++x; }
来源：http://hz.snrcjt.cn/gtibarrisn.html


<!-- 参考信息 -->