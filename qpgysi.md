代发 wailian999

[Q67] 设置隔离级别
来源：http://hz.zhixingplan.top/gtjrhcdzjq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cucudq.cn/gtrzlspuzu.html

[Q68] 保存点
来源：http://hz.chenjidiqi.icu/gtktamgqny.html

SAVEPOINT sp1;
来源：http://hz.redwolf501.top/gtdvmostiy.html

ROLLBACK TO sp1;
来源：http://hz.xingfuxueyuan.xyz/gtoowdqcom.html

[Q69] 查看执行计划
来源：http://hz.aibaodan.cn/gtuttworqi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jiagoushi.top/gtwytzshrc.html

[Q70] 更新统计信息
来源：http://hz.ppjwa.cn/gtpkniybgr.html

ANALYZE TABLE users;
来源：http://hz.quarkkingdee.top/gtgtgwpxxi.html

[Q71] 查看建表语句
来源：http://hz.haohaochexian.top/gtnskzmddv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.guannengcc.top/gtokdzbcfu.html

[Q72] 查看索引
来源：http://hz.feifeiyinyue.top/gtbcaemwyu.html

SHOW INDEX FROM users;
来源：http://hz.tianlin.xyz/gtqrbkjwip.html

[Q73] 查看表状态
来源：http://hz.yueranfly.top/gtejrgvysg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.xingfuxueyuan.xyz/gtfhliupto.html

[Q74] 强制使用索引
来源：http://hz.jinghuilouyu.cn/gtepglpxch.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhongyouzk.top/gtjkmgvxrv.html

[Q75] 日期格式化
来源：http://hz.chenjidiqi.icu/gtprspwizt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.0kj1m.cn/gttyocfkjs.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shuidangran.top/gtjfkfthny.html

[Q76] 按天统计
来源：http://hz.hnqzz.top/gtmtysovlv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.svipenyu.cn/gtsgicuvwn.html

[Q77] 时间加减
来源：http://hz.jyoumei.cn/gtllqbnuiu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.pengpengdd.cyou/gtqlkiynwl.html

[Q78] 当前时间
来源：http://hz.xinyue.icu/gtbgiknuyc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.gogol.net.cn/gtaoeebjyk.html

[Q79] 字符串拼接
来源：http://hz.aibaodan.cn/gtdyjfddch.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hfpthk.cn/gtpmenspds.html

[Q80] 字符串截取
来源：http://hz.shzxlz.cn/gtybasqqkz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.dianchejie.cn/gtpshzgiei.html

[Q81] 字符串替换
来源：http://hz.yj202588.top/gtbhbecjhw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.c1oappe.top/gtmwkcvnmo.html

[Q82] 字符长度与字节长度
来源：http://hz.xuanzx.com/gtdpjvxsnc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yj20258.top/gtzuwniuim.html

[Q83] 大小写转换
来源：http://hz.316326.xyz/gtsfsbidiz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hongshengwenyu.top/gtxikwrywx.html

[Q84] 去除首尾空格
来源：http://hz.hnxiangtu.top/gtdrrmugvu.html

SELECT TRIM(name) FROM users;
来源：http://hz.chenlongwang.top/gtgnbhgreq.html

[Q85] 数值取整
来源：http://hz.jinqigufen.top/gtevajddqj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.vqdsnc.cn/gthgqjijlu.html

[Q86] 读取 JSON 字段
来源：http://hz.sxryk.cn/gtcvlhgykw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.haohaochexian.top/gtmxnauyvi.html

[Q87] JSON 字段做条件
来源：http://hz.yj20258.top/gtnhwnpxze.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yonumen.top/gtmrefhtiw.html

[Q88] 行转列（条件聚合）
来源：http://hz.cqqwz.cn/gtreahoszg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hysaishi.cn/gtnjhlizjo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.gaohongyu789.top/gtxcdfzmwr.html

[Q89] 判断表是否存在
来源：http://hz.zhoulong.xyz/gtezxdkijh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.cucudq.cn/gtebtbtzhg.html

[Q90] 生成序号列
来源：http://hz.pycfn.com/gtizaeyvdz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ybcxt.top/gtoshlwlda.html

================================================================================
来源：http://hz.guannengcc.top/gtliefdeiw.html

R. Bash 专题
来源：http://hz.yonumen.top/gtnekklztk.html

================================================================================
来源：http://hz.jinqigfzy.top/gtojuxkush.html

[R01] shebang 与严格模式
来源：http://hz.wangshuangyany.cn/gtijsrgwdp.html

#!/usr/bin/env bash
来源：http://hz.smart0.xyz/gtljhxptwr.html

set -euo pipefail
来源：http://hz.daxiang520.top/gtfhxlydre.html

[R02] 变量赋值与使用
来源：http://hz.vqdsnc.cn/gtwekxytht.html

name="Tom"; echo "$name"
来源：http://hz.sufxvd.cn/gtciaxtgfz.html

[R03] 只读变量
来源：http://hz.jlsjyb.cn/gtvqcutspo.html

readonly PI=3.14
来源：http://hz.nanxinkj.top/gtihapizlg.html

[R04] 位置参数
来源：http://hz.yanxiufei.cn/gtwahvgfcw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ybcxt.top/gtiyqikqxl.html

[R05] 参数默认值
来源：http://hz.yj20258.top/gtwgwdqqmi.html

name="${1:-default}"
来源：http://hz.zdqjudy.top/gtsjgpwssu.html

[R06] 判断命令是否存在
来源：http://hz.ivvv.top/gtcpfljbmm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhongyouzk.top/gtuhaonqyt.html

[R07] if 判断文件
来源：http://hz.yongpay.top/gtosnobhyq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yuxming.cn/gtroptxsnn.html

[R08] 数值比较
来源：http://hz.ppjwa.cn/gtdzoniiya.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.mhx1999.top/gtyfcbnexv.html

[R09] 字符串比较
来源：http://hz.ywan-chungtsiang.top/gtxrpnmhqd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.bjfxy.top/gtorsyectb.html

[R10] 正则匹配
来源：http://hz.chenlongwang.top/gtzioqkdde.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xuetiantiany.cn/gtkkkjageu.html

[R11] case 多分支
来源：http://hz.gaohongyu789.top/gtelzoqdjz.html

case "$1" in
来源：http://hz.hongshengwenyu.top/gtefyhxbrx.html

start) echo "启动" ;;
来源：http://hz.guannengcc.top/gtxfmtnbvf.html

stop)  echo "停止" ;;
来源：http://hz.sufxvd.cn/gtgdvlizji.html

*)     echo "未知命令" ;;
来源：http://hz.zycfv.cn/gtvqbllvxg.html

esac
来源：http://hz.chenjidiqi.icu/gtlucpvklv.html

[R12] for 遍历文件
来源：http://hz.yongpay.top/gtxduxbgmt.html

for f in *.txt; do echo "$f"; done
来源：http://hz.birdmap.top/gtkuuticks.html

[R13] for 计数循环
来源：http://hz.gogol.net.cn/gtyogmvesy.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jqgfzy.top/gtiyujjvmp.html

[R14] C 风格 for
来源：http://hz.cucudq.cn/gtqulpqfwg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhijiandao.cn/gtcmyoyyiz.html

[R15] while 逐行读文件
来源：http://hz.jinqigfzy.top/gtdkznvnlw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jqgufenzy.top/gtlkymacxi.html

[R16] until 等待条件
来源：http://hz.redwolf501.top/gtkwjiieqz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.wangdashe.top/gtcryunkkx.html

[R17] 数组定义与取值
来源：http://hz.yonumen.top/gtigdzvlnj.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yonumen.top/gtzecnayyv.html

[R18] 遍历数组
来源：http://hz.birdmap.top/gtwveslnso.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ydjk.org.cn/gtzgolsqao.html

[R19] 数组长度
来源：http://hz.jinqigufen.top/gthmvytprx.html

echo "${#arr[@]}"
来源：http://hz.zhaomingkeji.xyz/gtvawhidzd.html

[R20] 关联数组（字典）
来源：http://hz.zhengqikj.top/gtopevcqqi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hywenlv.cn/gtzxprfoky.html

[R21] 字符串长度
来源：http://hz.gotoacloud.top/gtikjgbkds.html

echo "${#s}"
来源：http://hz.zhijiandao.cn/gtutrxjivw.html

[R22] 截取子串
来源：http://hz.cqqwz.cn/gtmcnncgbk.html

echo "${s:0:5}"
来源：http://hz.tanke756.top/gtszuicqwy.html

[R23] 字符串替换
来源：http://hz.yonumen.top/gtpddhgxid.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ywan-chungtsiang.top/gtncbdqsnz.html

[R24] 大小写转换
来源：http://hz.gogol.net.cn/gtudojlgmi.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shangyingyoupin.top/gtkcduwodi.html

[R25] 去后缀 / 去前缀
来源：http://hz.tanke756.top/gtetrligcw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.haohaochexian.top/gtjnjwnyjw.html

[R26] 命令替换
来源：http://hz.jlsjyb.cn/gtdxxzclgp.html

now=$(date +%F); echo "$now"
来源：http://hz.zhoulong.xyz/gtfhlbitvo.html

[R27] 算术展开
来源：http://hz.gzhubu.top/gtuquyzfnf.html

echo $((1 + 2 * 3))
来源：http://hz.chenlongwang.top/gtiwcofyba.html

[R28] 浮点运算
来源：http://hz.daria6918.cn/gteqbkcdfo.html

echo "scale=2; 10/3" | bc
来源：http://hz.hysaishi.cn/gtvgapflen.html

[R29] 定义函数
来源：http://hz.52xcode.cn/gtskdrfwlh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yuxming.cn/gtatuqswlz.html

[R30] 函数返回状态码
来源：http://hz.shangyingyoupin.top/gtiuocbycg.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.wangshuangyany.cn/gtngbkbmwm.html

[R31] 局部变量
来源：http://hz.hnxiangtu.top/gtcqzlharh.html

f() { local x=1; echo "$x"; }
来源：http://hz.0kj1m.cn/gtplvygyvj.html

[R32] 参数个数校验
来源：http://hz.yueranfly.top/gtdioheyev.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.sufxvd.cn/gtsbnassma.html

[R33] 捕获错误并提示行号
来源：http://hz.jinqigufen.top/gtckczffqe.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhoulong.xyz/gtarxfndki.html

[R34] 退出时清理
来源：http://hz.shanyushiyangtech.top/gtdxtfxufo.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.52xcode.cn/gtmioyfxsg.html

[R35] 后台执行并等待
来源：http://hz.mhx1999.top/gtciqoqmmo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.316326.xyz/gtahcflpxq.html

[R36] 并发执行多个任务
来源：http://hz.haohaochexian.top/gteukbgggu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhongyouzk.top/gtcfymjixr.html

[R37] 把输出赋给变量
来源：http://hz.gogol.net.cn/gtkqkryrhm.html

files=$(ls -1)
来源：http://hz.ppjwa.cn/gtmmpbhntb.html

[R38] 管道串联
来源：http://hz.ehwqpu.com/gtvqldluuc.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ehwqpu.com/gthjkzwucz.html

[R39] 重定向标准输出与错误
来源：http://hz.316326.xyz/gtwefrbunh.html

cmd > out.log 2>&1
来源：http://hz.zdqjudy.top/gtsvmozrnz.html

[R40] 追加写日志
来源：http://hz.jlsjyb.cn/gtpwgavfxn.html

echo "log" >> out.log
来源：http://hz.guowangkeji.top/gtmvtrrnaj.html

[R41] 丢弃输出
来源：http://hz.ydjk.org.cn/gtjhpwccyv.html

cmd >/dev/null 2>&1
来源：http://hz.nanxinkj.top/gtuqyzezka.html

[R42] 输入重定向
来源：http://hz.redwolf501.top/gtkhilkjqu.html

wc -l < a.txt
来源：http://hz.yanxiufei.cn/gtgwbnxnku.html

[R43] 按名字查找文件
来源：http://hz.yuanzhike.top/gttrdhlzqz.html

find . -name "*.log" -type f
来源：http://hz.jinqigufen.top/gtjabrgliv.html

[R44] 按修改时间查找
来源：http://hz.chenlongwang.top/gtzjppuzpc.html

find . -mtime -7 -type f
来源：http://hz.mhx1999.top/gthwjkwdtm.html

[R45] 批量删除
来源：http://hz.0kj1m.cn/gtuuueqcrq.html

find . -name "*.tmp" -delete
来源：http://hz.yangfankeji.com/gtyojchbsv.html

[R46] 递归替换文件内容
来源：http://hz.yueranfly.top/gtlkqxajjs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shangyingyoupin.top/gtlvqudebn.html

[R47] sed 单行替换
来源：http://hz.jinqigufen.top/gtrgqyyzds.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xylfe.cn/gtdvgjlttl.html

[R48] awk 取指定列
来源：http://hz.mhx1999.top/gtirbjeqri.html

awk '{print $1, $3}' a.txt
来源：http://hz.wangdashe.top/gtibfzxoji.html

[R49] awk 带条件
来源：http://hz.xuetiantiany.cn/gtawygdlne.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jyoumei.cn/gtdpfutpnw.html

[R50] awk 求和
来源：http://hz.xingfuxueyuan.xyz/gtobtcjrbi.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xuanzx.com/gtctsgpfbr.html

[R51] 排序去重取前几
来源：http://hz.yongpay.top/gtvlinqpwx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.tianlin.xyz/gtywgwveyi.html

[R52] 统计行数
来源：http://hz.xuetiantiany.cn/gtuxasmzsr.html

wc -l a.txt
来源：http://hz.quarkkingdee.top/gtiokhjvlh.html

[R53] 查看文件头与实时尾
来源：http://hz.haohaochexian.top/gtektyezep.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shangyingyoupin.top/gttguluueo.html

[R54] 比较两个文件
来源：http://hz.daria6918.cn/gtzzvhnfpa.html

diff a.txt b.txt
来源：http://hz.shzxlz.cn/gtqragbgju.html

[R55] 压缩与解压
来源：http://hz.yuxming.cn/gtucgdauck.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.sxryk.cn/gtyrzddcjg.html

[R56] 远程拷贝
来源：http://hz.zhixingplan.top/gtfsqnvdnh.html

scp file user@host:/path/
来源：http://hz.zhijiandao.cn/gtrqnpdmll.html

[R57] 远程执行命令
来源：http://hz.daria6918.cn/gtfyvtrycw.html

ssh user@host 'uptime'
来源：http://hz.zhixingplan.top/gtgyqvthnw.html

[R58] 下载文件
来源：http://hz.hammf.cn/gtptbovyon.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.guowangkeji.top/gtvkgbgeba.html

[R59] 发 POST JSON
来源：http://hz.chenzaomai.com/gtmqxvpvwv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.aibaodan.cn/gtkpkjsxqi.html

[R60] 只看 HTTP 状态码
来源：http://hz.yongpay.top/gttfrrbiez.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yonumen.top/gtguxupjdb.html

[R61] 磁盘占用
来源：http://hz.gaohongyu789.top/gtlcanvcxw.html

df -h;  du -sh *
来源：http://hz.c1oappe.top/gtmidfatnt.html

[R62] 找最占空间的文件
来源：http://hz.redwolf501.top/gtjucdtlew.html

du -ah . | sort -rh | head -10
来源：http://hz.svipenyu.cn/gtlgfhivrc.html

[R63] 内存与进程
来源：http://hz.yonumen.top/gtncmpqkqe.html

free -h;  ps aux | grep nginx
来源：http://hz.fengsongda.top/gtdyciiqth.html

[R64] 结束进程
来源：http://hz.shanyushiyangtech.top/gtftjwmexd.html

kill -9 $(pgrep -f app.py)
来源：http://hz.smart0.xyz/gtdbflsagl.html

[R65] 查看端口占用
来源：http://hz.chenlongwang.top/gtbuwuivmg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yuanzhike.top/gtzsyksmkv.html

[R66] 定时任务
来源：http://hz.meibo888.top/gtlzimhood.html

crontab -e;  crontab -l
来源：http://hz.nanxuanxn.top/gtigodncbm.html

[R67] 生成随机十六进制串
来源：http://hz.yangfankeji.com/gtjsicjbms.html

openssl rand -hex 16
来源：http://hz.0kj1m.cn/gtknxkdsry.html

[R68] 计算文件校验值
来源：http://hz.nanxinkj.top/gtskrugewf.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.gaohongyu789.top/gtoycqrfsv.html

[R69] 生成随机密码
来源：http://hz.316326.xyz/gtodgvuiqq.html

head -c 16 /dev/urandom | base64
来源：http://hz.c1oappe.top/gtcbfseyak.html

[R70] 时间戳与互转
来源：http://hz.gzhubu.top/gtpsjzzbrp.html

date +%s;  date -d @1700000000
来源：http://hz.xinyue.icu/gteowemqxf.html

[R71] 日期格式化
来源：http://hz.jianghu66.top/gtybwpohgq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hongshengwenyu.top/gtlgjgnmmi.html

[R72] 等待端口就绪
来源：http://hz.smart0.xyz/gtzwtlsjfw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hnqzz.top/gtadvginyw.html

[R73] 分割大日志
来源：http://hz.nanxinkj.top/gtdtokrnfl.html

split -l 1000 big.log part_
来源：http://hz.tianlin.xyz/gtmdnyqetz.html

[R74] 批量重命名
来源：http://hz.xuanzx.com/gtxxqwbhhe.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cashguo.top/gtrogytydo.html

[R75] 导出环境变量
来源：http://hz.cqqwz.cn/gtsalakxpa.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yj20258888.top/gtxviejtow.html

[R76] 使用临时文件
来源：http://hz.yuxming.cn/gtnsdokhry.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xziqi.cn/gtffnyvylh.html

[R77] 读取用户输入
来源：http://hz.jinghuilouyu.cn/gtgngqozdp.html

read -rp "请输入: " ans
来源：http://hz.jinyuanbaomall.cn/gtrzxvarni.html

[R78] 交互式菜单
来源：http://hz.shanyushiyangtech.top/gtvdzupczj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.nwbrower.top/gtxxuboddd.html

[R79] 解析命令行选项
来源：http://hz.jlsjyb.cn/gtnlstxybl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.9152youxi.cn/gtxwvsqjml.html

[R80] 查看脚本执行耗时
来源：http://hz.zhongyouzk.top/gtxnivusgl.html

time ./run.sh
来源：http://hz.jqgufenzy.top/gtlopsyxcl.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtrhkuubvm.html

S. C / C++ 专题
来源：http://hz.yonumen.top/gtflxfxuzj.html

================================================================================
来源：http://hz.tianlin.xyz/gtxdfeoven.html

[S01] C：Hello World
来源：http://hz.smart0.xyz/gtraepnchi.html

#include <stdio.h>
来源：http://hz.zhengqikj.top/gtiwvmhztg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.aizwys.cn/gtzyicrgpi.html

[S02] C：变量与格式化输出
来源：http://hz.guannengcc.top/gthsvozeem.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhiwuduotai.top/gtslxjnqjd.html

[S03] C：读入整数
来源：http://hz.sysykeji.top/gtkhmjwykr.html

int x; scanf("%d", &x);
来源：http://hz.bjfxy.top/gtnmkmjlzi.html

[S04] C：字符串复制
来源：http://hz.yvedp.cn/gtctsdjlqx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.meibo888.top/gtdzxuoknn.html

[S05] C：字符串长度
来源：http://hz.redwolf501.top/gtozljhinr.html

strlen(s)
来源：http://hz.havefunace.top/gtzjtwspce.html

[S06] C：字符串比较
来源：http://hz.ywan-chungtsiang.top/gttkmqlfaj.html

strcmp(a, b) == 0
来源：http://hz.sweek.top/gtxirfesip.html

[S07] C：数组遍历求和
来源：http://hz.havefunace.top/gtvjpxryac.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ydzc1.top/gtyfqbcbcy.html

[S08] C：动态内存分配与释放
来源：http://hz.jqgufenzy.top/gtovsmybbd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.wangshuangyany.cn/gtevbrqmiu.html

[S09] C：结构体定义与初始化
来源：http://hz.hnqzz.top/gtfqxtlswh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.vqdsnc.cn/gtwtuuuipw.html

[S10] C：指针与解引用
来源：http://hz.ydzc1.top/gtmytveokp.html

int *p = &a;  *p = 5;
来源：http://hz.kuanghao11.cn/gtcrizwxvq.html

[S11] C：逐行读文件
来源：http://hz.chenjidiqi.icu/gtdbytyexn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.havefunace.top/gtfggqhkvv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hfpthk.cn/gtkfcgntne.html

fclose(f);
来源：http://hz.sxryk.cn/gtckzcidrd.html

[S12] C：写文件
来源：http://hz.yj20258.top/gtkxqgnqge.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jinghuilouyu.cn/gtbobrynhb.html

[S13] C：宏定义
来源：http://hz.andypj.xyz/gtyhdwczxw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.tian-w.cn/gtglwcwapz.html

[S14] C：枚举
来源：http://hz.vqdsnc.cn/gtqmafaksu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.kuanghao11.cn/gtnsxsvuch.html

[S15] C：类型转换
来源：http://hz.shangyingyoupin.top/gtblsdgqdr.html

(double) a / b
来源：http://hz.wangshuangyany.cn/gtvmfdpqgd.html

[S16] C：位操作置位
来源：http://hz.ivvv.top/gtjvhkwcqh.html

x |= (1 << 3);
来源：http://hz.zdqjudy.top/gtojceglxt.html

[S17] C：安全拼接字符串
来源：http://hz.yuxming.cn/gtsodawiea.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.chenlongwang.top/gtsissokbc.html

[S18] C：命令行参数
来源：http://hz.xingfuxueyuan.xyz/gtzhmttkkz.html

int main(int argc, char **argv)
来源：http://hz.vqdsnc.cn/gthwqmdzev.html

[S19] C：快速排序
来源：http://hz.gogol.net.cn/gtcidzyobi.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ehwqpu.com/gtgnsfgrkm.html

[S20] C：二分查找
来源：http://hz.quarkkingdee.top/gtytzyuesa.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xziqi.cn/gtomjalmxv.html

[S21] C：字符类别判断
来源：http://hz.tian-w.cn/gthrncyrjr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.andypj.xyz/gthkvnjrqj.html

[S22] C：字符串转数字
来源：http://hz.sufxvd.cn/gtnblglxss.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shanyushiyangkeji.top/gtcedmhawj.html

[S23] C：随机数
来源：http://hz.hnqzz.top/gtjiqcpdnb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.haohaochexian.top/gtaxfbplst.html

[S24] C：获取本地时间
来源：http://hz.yj202588.top/gtifhrclrb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hongshengwenyu.top/gtdzkfqlcx.html

[S25] C：内存拷贝
来源：http://hz.zhixingplan.top/gtpaxmnwgd.html

memcpy(dst, src, n);
来源：http://hz.gotoacloud.top/gtmyojkqyx.html

[S26] C：内存清零
来源：http://hz.mhx1999.top/gtomsbmdgo.html

memset(a, 0, sizeof a);
来源：http://hz.yj202588.top/gtkyebutsi.html

[S27] C：定义常量
来源：http://hz.daria6918.cn/gtsnqtczvj.html

const double PI = 3.14159;
来源：http://hz.vqdsnc.cn/gtqvpijpzl.html

[S28] C：静态变量
来源：http://hz.andypj.xyz/gtoudwcjxr.html

static int counter = 0;
来源：http://hz.hongshengwenyu.top/gtkrspxwhg.html

[S29] C：变参函数
来源：http://hz.jiagoushi.top/gtymzybkfo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shanyushiyangkeji.top/gtbuuajcec.html

[S30] C：头文件保护
来源：http://hz.shanyushiyangtech.top/gtptctccxt.html

#ifndef X_H
来源：http://hz.jianghu66.top/gtohiceoll.html

#define X_H
来源：http://hz.xinyue.icu/gttrqgtnwz.html

#endif
来源：http://hz.birdmap.top/gthuaaatph.html

[S31] C++：Hello World
来源：http://hz.pengpengdd.cyou/gtmsiwtbfs.html

#include <iostream>
来源：http://hz.shanyushiyangtech.top/gtyhwrjvwv.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jyoumei.cn/gtgvownvix.html

[S32] C++：字符串
来源：http://hz.yonumen.top/gtysmqfuau.html

std::string s = "hi";  s += "!";
来源：http://hz.zhijiandao.cn/gtpesstefb.html

[S33] C++：vector 增删
来源：http://hz.redwolf501.top/gtabybjrqz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ehwqpu.com/gtfbqvgsrn.html

[S34] C++：遍历 vector
来源：http://hz.sufxvd.cn/gtrkebnhym.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.wangdashe.top/gtsodqjmqy.html

[S35] C++：map
来源：http://hz.shzxlz.cn/gtwasidfvt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pengpengdd.cyou/gtkpscejhf.html

[S36] C++：unordered_map
来源：http://hz.jqgfzy.top/gtqwrgmbwi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.andypj.xyz/gtlhtltmsi.html


<!-- 参考信息 -->