代发 wailian999

ROLLBACK TO sp1;
来源：http://hz.jqgufenzy.top/gtiwxlnemk.html

[Q69] 查看执行计划
来源：http://hz.sysykeji.top/gtninufvki.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jinyuanbaomall.cn/gtwtwwuwfx.html

[Q70] 更新统计信息
来源：http://hz.smart0.xyz/gtwumaolau.html

ANALYZE TABLE users;
来源：http://hz.xinyue.icu/gtzfnasnln.html

[Q71] 查看建表语句
来源：http://hz.ehwqpu.com/gtkaugmbum.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.dianchejie.cn/gtnawnibfr.html

[Q72] 查看索引
来源：http://hz.jlsjyb.cn/gtcduryfyd.html

SHOW INDEX FROM users;
来源：http://hz.ydjk.org.cn/gtxxrbelwc.html

[Q73] 查看表状态
来源：http://hz.c1oappe.top/gtyttpcfly.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hnqzz.top/gtammnkhqn.html

[Q74] 强制使用索引
来源：http://hz.zhijiandao.cn/gtawhqxsbp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.vqdsnc.cn/gtlsnttmww.html

[Q75] 日期格式化
来源：http://hz.dianchejie.cn/gtomyefsms.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhijiandao.cn/gtxrhtdsjn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.fzhhl.top/gtyumugvel.html

[Q76] 按天统计
来源：http://hz.fengsongda.top/gteqddaxtt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shanyushiyangtech.top/gtmuhtoiml.html

[Q77] 时间加减
来源：http://hz.jyoumei.cn/gtguhtjwqr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nanxuanxn.top/gteltdxeat.html

[Q78] 当前时间
来源：http://hz.yvedp.cn/gtjukxawyp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.9152youxi.cn/gttcsrjwtd.html

[Q79] 字符串拼接
来源：http://hz.jyoumei.cn/gtxtygxbdo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zycfv.cn/gtxlgibbad.html

[Q80] 字符串截取
来源：http://hz.gotoacloud.top/gttxvxwobd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.wangdashe.top/gthldsaada.html

[Q81] 字符串替换
来源：http://hz.cucudq.cn/gtpnmswcva.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ydjk.org.cn/gtzwdejijs.html

[Q82] 字符长度与字节长度
来源：http://hz.yuxming.cn/gtzbyvihqy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.gogol.net.cn/gtcjonjsgn.html

[Q83] 大小写转换
来源：http://hz.shuidangran.top/gtpwzknvfk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.mhx1999.top/gtyitfgpzp.html

[Q84] 去除首尾空格
来源：http://hz.52xcode.cn/gtsnoqjcuo.html

SELECT TRIM(name) FROM users;
来源：http://hz.nwbrower.top/gtqjkgxoru.html

[Q85] 数值取整
来源：http://hz.aibaodan.cn/gtkjbeorxk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.guannengcc.top/gtzexjmazj.html

[Q86] 读取 JSON 字段
来源：http://hz.tanke756.top/gtbkbylvzf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhengqikj.top/gtcunfauwr.html

[Q87] JSON 字段做条件
来源：http://hz.jqgfzy.top/gttweuiaek.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.0kj1m.cn/gtewfttqjb.html

[Q88] 行转列（条件聚合）
来源：http://hz.aibaodan.cn/gtpciooyyn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ehwqpu.com/gtramunurc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.sysykeji.top/gthyuaopqu.html

[Q89] 判断表是否存在
来源：http://hz.zycfv.cn/gtxemmdcah.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.316326.xyz/gtrckuwqfj.html

[Q90] 生成序号列
来源：http://hz.jinqigfzy.top/gtkfgerrjb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yanxiufei.cn/gtuynxfuhi.html

================================================================================
来源：http://hz.chenzaomai.com/gtplenixob.html

R. Bash 专题
来源：http://hz.zhoulong.xyz/gtedganwqf.html

================================================================================
来源：http://hz.xylfe.cn/gttcwcsefq.html

[R01] shebang 与严格模式
来源：http://hz.xuanzx.com/gtimtxvogz.html

#!/usr/bin/env bash
来源：http://hz.zhongyouzk.top/gtbxpvhhar.html

set -euo pipefail
来源：http://hz.ivvv.top/gtqjwgmohu.html

[R02] 变量赋值与使用
来源：http://hz.quarkkingdee.top/gtwkjbaekp.html

name="Tom"; echo "$name"
来源：http://hz.feifeiyinyue.top/gtrfezmeqt.html

[R03] 只读变量
来源：http://hz.iojbl.cn/gtjcvsvhem.html

readonly PI=3.14
来源：http://hz.haohaochexian.top/gtgxtyedmk.html

[R04] 位置参数
来源：http://hz.zdqjudy.top/gtxdiqbhty.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.0kj1m.cn/gttzrfimpw.html

[R05] 参数默认值
来源：http://hz.ybcxt.top/gtltwpogfx.html

name="${1:-default}"
来源：http://hz.cqqwz.cn/gtzrkqnefu.html

[R06] 判断命令是否存在
来源：http://hz.gotoacloud.top/gtiehruqwp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.wangshuangyany.cn/gtrcdcttgp.html

[R07] if 判断文件
来源：http://hz.yj20258.top/gtmybcpokr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.fzhhl.top/gtgbzaetlb.html

[R08] 数值比较
来源：http://hz.yj20258888.top/gteonhhvfz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yanxiufei.cn/gtcqnkrvki.html

[R09] 字符串比较
来源：http://hz.gaohongyu789.top/gtgchpkrgs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shangyingyoupin.top/gtlwvoigyw.html

[R10] 正则匹配
来源：http://hz.gzhubu.top/gterdpfwux.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.daxiang520.top/gthqybibmk.html

[R11] case 多分支
来源：http://hz.yueranfly.top/gtlsalcvgj.html

case "$1" in
来源：http://hz.jqgufenzy.top/gtmacjhmff.html

start) echo "启动" ;;
来源：http://hz.zhoulong.xyz/gtdwuziekg.html

stop)  echo "停止" ;;
来源：http://hz.yueranfly.top/gttfewtssq.html

*)     echo "未知命令" ;;
来源：http://hz.pengpengdd.cyou/gtafpqcbhl.html

esac
来源：http://hz.sufxvd.cn/gtecezruva.html

[R12] for 遍历文件
来源：http://hz.shuidangran.top/gtyhvtxrxz.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hnxiangtu.top/gtljjlakrg.html

[R13] for 计数循环
来源：http://hz.yanxiufei.cn/gtcamqzdaw.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cucudq.cn/gtxypctsoo.html

[R14] C 风格 for
来源：http://hz.gotoacloud.top/gtrslrrmnc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhaomingkeji.xyz/gtaphkegio.html

[R15] while 逐行读文件
来源：http://hz.xuanzx.com/gtvnzxajli.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.daxiang520.top/gtwinkqrns.html

[R16] until 等待条件
来源：http://hz.jqgfzy.top/gtdekjguhj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jyoumei.cn/gtftppjrcj.html

[R17] 数组定义与取值
来源：http://hz.9152youxi.cn/gtntqxpmob.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yj20258.top/gtlzcjjoka.html

[R18] 遍历数组
来源：http://hz.52xcode.cn/gtqqhanagl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xuetiantiany.cn/gtsjostzyf.html

[R19] 数组长度
来源：http://hz.cdnleiting.top/gtkpjryowy.html

echo "${#arr[@]}"
来源：http://hz.zhiwuduotai.top/gtvkjgbhxr.html

[R20] 关联数组（字典）
来源：http://hz.xuetiantiany.cn/gtijtvjjvc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yonumen.top/gtdnvtptnv.html

[R21] 字符串长度
来源：http://hz.nanxinkj.top/gtkwrfcrll.html

echo "${#s}"
来源：http://hz.cheryme.top/gtytwlyqrl.html

[R22] 截取子串
来源：http://hz.snrcjt.cn/gtflyczveb.html

echo "${s:0:5}"
来源：http://hz.gzhubu.top/gtdxpgaexo.html

[R23] 字符串替换
来源：http://hz.yangfankeji.com/gtigdyqqkb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.redwolf501.top/gtyzmdzkrl.html

[R24] 大小写转换
来源：http://hz.yj20258.top/gtkkdppfmo.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.guowangkeji.top/gtclrxmhle.html

[R25] 去后缀 / 去前缀
来源：http://hz.hammf.cn/gthzvrtlrg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhiwuduotai.top/gtrutyeysp.html

[R26] 命令替换
来源：http://hz.hfpthk.cn/gtubprqovq.html

now=$(date +%F); echo "$now"
来源：http://hz.gogol.net.cn/gtqyyecpjf.html

[R27] 算术展开
来源：http://hz.hongshengwenyu.top/gtlxniibkt.html

echo $((1 + 2 * 3))
来源：http://hz.svipenyu.cn/gtblwsbwwi.html

[R28] 浮点运算
来源：http://hz.0kj1m.cn/gtbtoqftlp.html

echo "scale=2; 10/3" | bc
来源：http://hz.chenzaomai.com/gtunwsqjqt.html

[R29] 定义函数
来源：http://hz.jqgfzy.top/gtgftdlcyi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hysaishi.cn/gtovbkgcyt.html

[R30] 函数返回状态码
来源：http://hz.jlsjyb.cn/gtxvqhwdoc.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.pengpengdd.cyou/gtkxyoxkkh.html

[R31] 局部变量
来源：http://hz.sysykeji.top/gtidchecgl.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhengqikj.top/gtjobfrovl.html

[R32] 参数个数校验
来源：http://hz.0kj1m.cn/gttbmswljn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ivvv.top/gtvuzssipz.html

[R33] 捕获错误并提示行号
来源：http://hz.ybcxt.top/gttjvycflb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xinyue.icu/gtuhtuyebo.html

[R34] 退出时清理
来源：http://hz.shzxlz.cn/gthskdhbhg.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.guowangkeji.top/gtewcnzxgq.html

[R35] 后台执行并等待
来源：http://hz.yj202588.top/gtjnqxcwdo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.guannengcc.top/gtblhostaa.html

[R36] 并发执行多个任务
来源：http://hz.snrcjt.cn/gtgydvgncn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.fzhhl.top/gtgyvsxrxh.html

[R37] 把输出赋给变量
来源：http://hz.sufxvd.cn/gtkarvzafb.html

files=$(ls -1)
来源：http://hz.yongpay.top/gtbvmjjfqf.html

[R38] 管道串联
来源：http://hz.zhijiandao.cn/gtwueyrqwi.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhixingplan.top/gtjulbbyes.html

[R39] 重定向标准输出与错误
来源：http://hz.ywan-chungtsiang.top/gtmmjyznnl.html

cmd > out.log 2>&1
来源：http://hz.sxryk.cn/gtmxjawzbq.html

[R40] 追加写日志
来源：http://hz.c1oappe.top/gtlwswmhir.html

echo "log" >> out.log
来源：http://hz.yuxming.cn/gtstzmwifv.html

[R41] 丢弃输出
来源：http://hz.smart0.xyz/gtymachafy.html

cmd >/dev/null 2>&1
来源：http://hz.fengsongda.top/gtdzyzytgb.html

[R42] 输入重定向
来源：http://hz.zdqjudy.top/gtiotiaiwn.html

wc -l < a.txt
来源：http://hz.yj20258.top/gtghrjrsnj.html

[R43] 按名字查找文件
来源：http://hz.jiagoushi.top/gtigqnqwgi.html

find . -name "*.log" -type f
来源：http://hz.c1oappe.top/gtmktlujmu.html

[R44] 按修改时间查找
来源：http://hz.iojbl.cn/gtfuymvbwj.html

find . -mtime -7 -type f
来源：http://hz.52xcode.cn/gtxvuduyxu.html

[R45] 批量删除
来源：http://hz.zhongyouzk.top/gtiehltnoj.html

find . -name "*.tmp" -delete
来源：http://hz.cdnleiting.top/gtltqirgpu.html

[R46] 递归替换文件内容
来源：http://hz.sweek.top/gthjrhefta.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jinyuanbaomall.cn/gtebfjzlvm.html

[R47] sed 单行替换
来源：http://hz.pycfn.com/gtnccyivlh.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jinghuilouyu.cn/gtexhpzxcn.html

[R48] awk 取指定列
来源：http://hz.tianlin.xyz/gttktffpyh.html

awk '{print $1, $3}' a.txt
来源：http://hz.feifeiyinyue.top/gtnhlqpkcp.html

[R49] awk 带条件
来源：http://hz.quarkkingdee.top/gtcifkijoh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.gotoacloud.top/gtfudgcpoj.html

[R50] awk 求和
来源：http://hz.316326.xyz/gtarubhoqr.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.tanke756.top/gtvqgpirwm.html

[R51] 排序去重取前几
来源：http://hz.xylfe.cn/gtlnakbedc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.9152youxi.cn/gtqkckndfs.html

[R52] 统计行数
来源：http://hz.cqqwz.cn/gtgbuvwimr.html

wc -l a.txt
来源：http://hz.guowangkeji.top/gtorbmjhsc.html

[R53] 查看文件头与实时尾
来源：http://hz.ydzc1.top/gtvcgdyhxc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yj20258.top/gtmxlrvddx.html

[R54] 比较两个文件
来源：http://hz.ydzc1.top/gtzzmnoffy.html

diff a.txt b.txt
来源：http://hz.shangyingyoupin.top/gtektqzumz.html

[R55] 压缩与解压
来源：http://hz.redwolf501.top/gtsshgiqcr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hongshengwenyu.top/gtqsrrbxmd.html

[R56] 远程拷贝
来源：http://hz.zycfv.cn/gtfgpsrqio.html

scp file user@host:/path/
来源：http://hz.feifeiyinyue.top/gtwuybuquw.html

[R57] 远程执行命令
来源：http://hz.c1oappe.top/gtfwutwsrd.html

ssh user@host 'uptime'
来源：http://hz.wangshuangyany.cn/gtlkwgmwzq.html

[R58] 下载文件
来源：http://hz.svipenyu.cn/gtnkgitogl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinyuanbaomall.cn/gtzjpiawzv.html

[R59] 发 POST JSON
来源：http://hz.shzxlz.cn/gtcjamklwb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.sweek.top/gtkvdosjqh.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhongyouzk.top/gtmnuahaef.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yuxming.cn/gtguadrlot.html

[R61] 磁盘占用
来源：http://hz.jqgufenzy.top/gtwzgrurkd.html

df -h;  du -sh *
来源：http://hz.shanyushiyangkeji.top/gttfqwhnup.html

[R62] 找最占空间的文件
来源：http://hz.aibaodan.cn/gteoclnixn.html

du -ah . | sort -rh | head -10
来源：http://hz.yangfankeji.com/gtwtyxcfyk.html

[R63] 内存与进程
来源：http://hz.birdmap.top/gtzwsnctwv.html

free -h;  ps aux | grep nginx
来源：http://hz.mhx1999.top/gthkdmquri.html

[R64] 结束进程
来源：http://hz.aibaodan.cn/gtaxnpxxfd.html

kill -9 $(pgrep -f app.py)
来源：http://hz.feifeiyinyue.top/gtjfhzrtfm.html

[R65] 查看端口占用
来源：http://hz.cdnleiting.top/gtassiwbwc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hnqzz.top/gtgnowfcgj.html

[R66] 定时任务
来源：http://hz.316326.xyz/gtijsleuoo.html

crontab -e;  crontab -l
来源：http://hz.dianchejie.cn/gtwdqdrtxf.html

[R67] 生成随机十六进制串
来源：http://hz.jinqigufen.top/gttmfpijhq.html

openssl rand -hex 16
来源：http://hz.tianlin.xyz/gtybwgrstk.html

[R68] 计算文件校验值
来源：http://hz.zdqjudy.top/gtkzvwrfsw.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.nanxinkj.top/gtqiljpuay.html

[R69] 生成随机密码
来源：http://hz.feifeiyinyue.top/gtsodvalbj.html

head -c 16 /dev/urandom | base64
来源：http://hz.shanyushiyangkeji.top/gthrffdpjc.html

[R70] 时间戳与互转
来源：http://hz.jqgfzy.top/gtewgpfmwv.html

date +%s;  date -d @1700000000
来源：http://hz.cashguo.top/gtusdexswq.html

[R71] 日期格式化
来源：http://hz.andypj.xyz/gtafprxwyd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xylfe.cn/gtigxwrcux.html

[R72] 等待端口就绪
来源：http://hz.ydzc1.top/gthegxvxzy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.sysykeji.top/gtokcaejxw.html

[R73] 分割大日志
来源：http://hz.guowangkeji.top/gtvfflzlcr.html

split -l 1000 big.log part_
来源：http://hz.fengsongda.top/gtaxdahvan.html

[R74] 批量重命名
来源：http://hz.shzxlz.cn/gtqjskmtwo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jianghu66.top/gtysbbazhj.html

[R75] 导出环境变量
来源：http://hz.haohaochexian.top/gtdpxqgucp.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ydjk.org.cn/gtqaonoole.html

[R76] 使用临时文件
来源：http://hz.pengpengdd.cyou/gttqqnsfaf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cdnleiting.top/gtgzcnomrv.html

[R77] 读取用户输入
来源：http://hz.cheryme.top/gtxtltrlzf.html

read -rp "请输入: " ans
来源：http://hz.smart0.xyz/gtsypgnznf.html

[R78] 交互式菜单
来源：http://hz.shanyushiyangtech.top/gtpsttineo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ppjwa.cn/gtdbyneywk.html

[R79] 解析命令行选项
来源：http://hz.zhoulong.xyz/gtviiuleun.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.daria6918.cn/gtfohbbcmo.html

[R80] 查看脚本执行耗时
来源：http://hz.xuanzx.com/gtvmfbcuhw.html

time ./run.sh
来源：http://hz.birdmap.top/gtolsxzwrn.html

================================================================================
来源：http://hz.vqdsnc.cn/gttaomvlph.html

S. C / C++ 专题
来源：http://hz.shanyushiyangtech.top/gtbimzaxqw.html

================================================================================
来源：http://hz.ivvv.top/gtdgsbhqos.html

[S01] C：Hello World
来源：http://hz.iojbl.cn/gtxsrljpuh.html

#include <stdio.h>
来源：http://hz.zdqjudy.top/gtikwptidd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.wangdashe.top/gtmjgpdkjs.html

[S02] C：变量与格式化输出
来源：http://hz.shangyingyoupin.top/gtmwohzjbm.html

int a = 10; printf("%d\n", a);
来源：http://hz.fengsongda.top/gtexxfprkq.html

[S03] C：读入整数
来源：http://hz.nanxuanxn.top/gthmrdidsp.html

int x; scanf("%d", &x);
来源：http://hz.dashuyun.cn/gtbonbwdwa.html

[S04] C：字符串复制
来源：http://hz.shanyushiyangtech.top/gtsghctzrm.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.aibaodan.cn/gtjqdxicri.html

[S05] C：字符串长度
来源：http://hz.ydzc1.top/gtabgdbqpa.html

strlen(s)
来源：http://hz.aibaodan.cn/gtkyfalkfk.html

[S06] C：字符串比较
来源：http://hz.sysykeji.top/gtbbwoblly.html

strcmp(a, b) == 0
来源：http://hz.quarkkingdee.top/gtfadrckal.html

[S07] C：数组遍历求和
来源：http://hz.nanxuanxn.top/gtzdezhtli.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ydjk.org.cn/gtefvdlwbw.html

[S08] C：动态内存分配与释放
来源：http://hz.gzhubu.top/gtbsdinpcq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jianghu66.top/gtuevydelm.html

[S09] C：结构体定义与初始化
来源：http://hz.jinqigfzy.top/gtmtsdtyph.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cqqwz.cn/gttstmssow.html

[S10] C：指针与解引用
来源：http://hz.ivvv.top/gtulkdjujs.html

int *p = &a;  *p = 5;
来源：http://hz.sufxvd.cn/gtidaofwcr.html

[S11] C：逐行读文件
来源：http://hz.redwolf501.top/gtojdeyrzh.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jinghuilouyu.cn/gtmocvzvly.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shanyushiyangkeji.top/gtbogrdeoq.html

fclose(f);
来源：http://hz.haohaochexian.top/gtqqextpcr.html

[S12] C：写文件
来源：http://hz.nanxinkj.top/gthgltcolb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yj20258.top/gtootoqylq.html

[S13] C：宏定义
来源：http://hz.hammf.cn/gtnbaaecbz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ydzc1.top/gtmjkequgu.html

[S14] C：枚举
来源：http://hz.ybcxt.top/gtixmtasck.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cashguo.top/gtdviquvvj.html

[S15] C：类型转换
来源：http://hz.dianchejie.cn/gtjbkftaoa.html

(double) a / b
来源：http://hz.nanxinkj.top/gtlkysspag.html

[S16] C：位操作置位
来源：http://hz.yj20258888.top/gtlzpebbev.html

x |= (1 << 3);
来源：http://hz.xuetiantiany.cn/gtnprvwnrf.html

[S17] C：安全拼接字符串
来源：http://hz.ywan-chungtsiang.top/gtisduolkt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.andypj.xyz/gtfwvunjtt.html

[S18] C：命令行参数
来源：http://hz.wangdashe.top/gtuhpfsasj.html

int main(int argc, char **argv)
来源：http://hz.xuanzx.com/gtkmzjtwou.html

[S19] C：快速排序
来源：http://hz.tianlin.xyz/gticwohwsy.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.c1oappe.top/gtjvnikqoy.html

[S20] C：二分查找
来源：http://hz.sysykeji.top/gtctcobaof.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.daxiang520.top/gtpxgccchz.html

[S21] C：字符类别判断
来源：http://hz.tian-w.cn/gtsqghqiyn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.snrcjt.cn/gtoknrtjel.html

[S22] C：字符串转数字
来源：http://hz.c1oappe.top/gtudfpgdif.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gogol.net.cn/gtoxlpwyaf.html

[S23] C：随机数
来源：http://hz.zhengqikj.top/gtapcmgqkw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.chenzaomai.com/gtkndqwqct.html

[S24] C：获取本地时间
来源：http://hz.yongpay.top/gttipbxsqz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.cqqwz.cn/gtvcceuqqy.html

[S25] C：内存拷贝
来源：http://hz.aizwys.cn/gtwbmeteby.html

memcpy(dst, src, n);
来源：http://hz.0kj1m.cn/gtmdoviyid.html

[S26] C：内存清零
来源：http://hz.hongshengwenyu.top/gtdgcpcpgt.html

memset(a, 0, sizeof a);
来源：http://hz.cdnleiting.top/gtzacqfivz.html

[S27] C：定义常量
来源：http://hz.jinqigufen.top/gtylztbfzb.html

const double PI = 3.14159;
来源：http://hz.feifeiyinyue.top/gtrpfeqhck.html

[S28] C：静态变量
来源：http://hz.zhongyouzk.top/gtuhsreoov.html

static int counter = 0;
来源：http://hz.zhaomingkeji.xyz/gtuukwidkl.html

[S29] C：变参函数
来源：http://hz.gogol.net.cn/gtuoevewav.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhengqikj.top/gtyimjhcot.html

[S30] C：头文件保护
来源：http://hz.aizwys.cn/gtkknlnbxd.html

#ifndef X_H
来源：http://hz.zhengqikj.top/gttqkcuunc.html

#define X_H
来源：http://hz.daxiang520.top/gtvnjmbxtf.html

#endif
来源：http://hz.haohaochexian.top/gtagwubocd.html

[S31] C++：Hello World
来源：http://hz.jqgufenzy.top/gtwvgcqscq.html

#include <iostream>
来源：http://hz.316326.xyz/gtgzojjfkj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.nanxuanxn.top/gtswtreaef.html

[S32] C++：字符串
来源：http://hz.quarkkingdee.top/gtxbcsgwdu.html

std::string s = "hi";  s += "!";
来源：http://hz.smart0.xyz/gtaqelijoi.html

[S33] C++：vector 增删
来源：http://hz.wangdashe.top/gtzsuxboki.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yj20258888.top/gtspgnjkot.html

[S34] C++：遍历 vector
来源：http://hz.redwolf501.top/gtggcgeeir.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jinqigfzy.top/gtclwoysib.html

[S35] C++：map
来源：http://hz.birdmap.top/gtoozadwhg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.birdmap.top/gtbpkldeqt.html

[S36] C++：unordered_map
来源：http://hz.havefunace.top/gtylnwvktt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.c1oappe.top/gthplqzkqm.html

[S37] C++：set
来源：http://hz.ehwqpu.com/gtholnrjtg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.nanxinkj.top/gtmwgeknzl.html

[S38] C++：排序
来源：http://hz.vqdsnc.cn/gtracwnmrl.html

std::sort(v.begin(), v.end());
来源：http://hz.gaohongyu789.top/gteuqfbsfx.html


<!-- 参考信息 -->