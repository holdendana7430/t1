代发 wailian999

[Q67] 设置隔离级别
来源：http://hz.yj202588.top/gtzvuqxgcm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.c1oappe.top/gtybabripw.html

[Q68] 保存点
来源：http://hz.andypj.xyz/gtqdtuxnmv.html

SAVEPOINT sp1;
来源：http://hz.yonumen.top/gtniilpzby.html

ROLLBACK TO sp1;
来源：http://hz.shuidangran.top/gtvzuyzhhs.html

[Q69] 查看执行计划
来源：http://hz.zycfv.cn/gttvrcthie.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yangfankeji.com/gtxmklslop.html

[Q70] 更新统计信息
来源：http://hz.vqdsnc.cn/gtuhvtpdkl.html

ANALYZE TABLE users;
来源：http://hz.chenjidiqi.icu/gtcdpuufir.html

[Q71] 查看建表语句
来源：http://hz.jqgufenzy.top/gtwsnmuqbq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.meibo888.top/gtukrcyjku.html

[Q72] 查看索引
来源：http://hz.yj20258888.top/gtsufynjqt.html

SHOW INDEX FROM users;
来源：http://hz.jinqigfzy.top/gtxdealnyw.html

[Q73] 查看表状态
来源：http://hz.jianghu66.top/gtkhmmjwag.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zycfv.cn/gtuxsxzwdj.html

[Q74] 强制使用索引
来源：http://hz.tian-w.cn/gtbzwcisbf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhiwuduotai.top/gtwareejed.html

[Q75] 日期格式化
来源：http://hz.cqqwz.cn/gtsdnuznjj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yanxiufei.cn/gtvxlbvwpk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hysaishi.cn/gtddlpiayn.html

[Q76] 按天统计
来源：http://hz.yongpay.top/gtvkdcdssf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yvedp.cn/gthsfroseg.html

[Q77] 时间加减
来源：http://hz.shanyushiyangkeji.top/gtmdarrsfl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.cdnleiting.top/gtlgpgrzwg.html

[Q78] 当前时间
来源：http://hz.xuetiantiany.cn/gtvdexozqp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.sufxvd.cn/gtburgawmw.html

[Q79] 字符串拼接
来源：http://hz.fengsongda.top/gtmmzhwqbf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yangfankeji.com/gtnqshpznk.html

[Q80] 字符串截取
来源：http://hz.jqgufenzy.top/gtfqqwgjyb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhixingplan.top/gtkwvesfnd.html

[Q81] 字符串替换
来源：http://hz.yangfankeji.com/gtnsxlqgot.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.gzhubu.top/gtuduwadry.html

[Q82] 字符长度与字节长度
来源：http://hz.yonumen.top/gtnuqkhvko.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xuetiantiany.cn/gtnsnudxwk.html

[Q83] 大小写转换
来源：http://hz.shanyushiyangtech.top/gteijqihnn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtjosyevcj.html

[Q84] 去除首尾空格
来源：http://hz.sweek.top/gthyjmpcib.html

SELECT TRIM(name) FROM users;
来源：http://hz.yongpay.top/gtmvtoqlus.html

[Q85] 数值取整
来源：http://hz.ivvv.top/gtzfahvdqm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yj20258.top/gttangpkav.html

[Q86] 读取 JSON 字段
来源：http://hz.ybcxt.top/gtznvwamyv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xuetiantiany.cn/gtfwtgtlve.html

[Q87] JSON 字段做条件
来源：http://hz.sxryk.cn/gtvyhzluyh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.0kj1m.cn/gttnssflze.html

[Q88] 行转列（条件聚合）
来源：http://hz.ybcxt.top/gtkaphvjbg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.tanke756.top/gthayavdnk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhijiandao.cn/gtcchgqawm.html

[Q89] 判断表是否存在
来源：http://hz.sxryk.cn/gttactvmxf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xingfuxueyuan.xyz/gtuwjerjtj.html

[Q90] 生成序号列
来源：http://hz.zycfv.cn/gtinceqrpm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shanyushiyangtech.top/gtjhgfpemi.html

================================================================================
来源：http://hz.zhixingplan.top/gtkzwtgeez.html

R. Bash 专题
来源：http://hz.hongshengwenyu.top/gtwqoqpxqa.html

================================================================================
来源：http://hz.meibo888.top/gtxsufuibi.html

[R01] shebang 与严格模式
来源：http://hz.jianghu66.top/gtrvfbcvwa.html

#!/usr/bin/env bash
来源：http://hz.gotoacloud.top/gtwgqeudwa.html

set -euo pipefail
来源：http://hz.shanyushiyangkeji.top/gtwgomgevk.html

[R02] 变量赋值与使用
来源：http://hz.guowangkeji.top/gtkxvictwe.html

name="Tom"; echo "$name"
来源：http://hz.hnqzz.top/gtptjoavcj.html

[R03] 只读变量
来源：http://hz.ydjk.org.cn/gtntfonogq.html

readonly PI=3.14
来源：http://hz.hfpthk.cn/gtriiktwos.html

[R04] 位置参数
来源：http://hz.gzhubu.top/gtadmgrmxn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.gzhubu.top/gtkbuvhstf.html

[R05] 参数默认值
来源：http://hz.sufxvd.cn/gtbtadpakx.html

name="${1:-default}"
来源：http://hz.jianghu66.top/gtkwwpgbxb.html

[R06] 判断命令是否存在
来源：http://hz.iojbl.cn/gtzwukowag.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shuidangran.top/gtkihftcrs.html

[R07] if 判断文件
来源：http://hz.hfpthk.cn/gtcmjeedam.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.iojbl.cn/gtjrhnoptc.html

[R08] 数值比较
来源：http://hz.gaohongyu789.top/gttnxvkpxv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhijiandao.cn/gtaqkgxubo.html

[R09] 字符串比较
来源：http://hz.hfpthk.cn/gtzwzhrlvw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.aizwys.cn/gtwpgnoxgj.html

[R10] 正则匹配
来源：http://hz.tian-w.cn/gtsvzagxfz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ppjwa.cn/gtvcjqygdq.html

[R11] case 多分支
来源：http://hz.guowangkeji.top/gtdcteimld.html

case "$1" in
来源：http://hz.jinqigufen.top/gtdjiqpddr.html

start) echo "启动" ;;
来源：http://hz.gzhubu.top/gtbaiqeabo.html

stop)  echo "停止" ;;
来源：http://hz.sysykeji.top/gtqxtilcyz.html

*)     echo "未知命令" ;;
来源：http://hz.shangyingyoupin.top/gttdawdrxw.html

esac
来源：http://hz.zhijiandao.cn/gtokvttifi.html

[R12] for 遍历文件
来源：http://hz.yj20258.top/gthmfcgomx.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yonumen.top/gtvkhkfmdm.html

[R13] for 计数循环
来源：http://hz.chenjidiqi.icu/gtoqzmcqiy.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shuidangran.top/gtwoihrzqh.html

[R14] C 风格 for
来源：http://hz.dianchejie.cn/gtahplssrc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jinghuilouyu.cn/gtdmihgmzp.html

[R15] while 逐行读文件
来源：http://hz.jinqigfzy.top/gtpzpvbwsv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.andypj.xyz/gtehbffcgp.html

[R16] until 等待条件
来源：http://hz.jqgufenzy.top/gtleegjyca.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ppjwa.cn/gtgaznyxdq.html

[R17] 数组定义与取值
来源：http://hz.ehwqpu.com/gtoyfgjydh.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.fzhhl.top/gtmifpsmpb.html

[R18] 遍历数组
来源：http://hz.snrcjt.cn/gtxzrzciju.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.wangshuangyany.cn/gtkvvqyjuj.html

[R19] 数组长度
来源：http://hz.jiagoushi.top/gtdduonznl.html

echo "${#arr[@]}"
来源：http://hz.gzhubu.top/gtdvhhbzww.html

[R20] 关联数组（字典）
来源：http://hz.aibaodan.cn/gtagimlrqr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhongyouzk.top/gtiqewzbhd.html

[R21] 字符串长度
来源：http://hz.shanyushiyangkeji.top/gtxnrxxfci.html

echo "${#s}"
来源：http://hz.sxryk.cn/gthgwtwica.html

[R22] 截取子串
来源：http://hz.aibaodan.cn/gtvhamcdyq.html

echo "${s:0:5}"
来源：http://hz.yuxming.cn/gtvdojetae.html

[R23] 字符串替换
来源：http://hz.yj20258.top/gtbupyhrrb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.andypj.xyz/gtdlithnih.html

[R24] 大小写转换
来源：http://hz.ppjwa.cn/gtlxguwkbb.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.aibaodan.cn/gtejfsxsja.html

[R25] 去后缀 / 去前缀
来源：http://hz.hnxiangtu.top/gthrpmndql.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hongshengwenyu.top/gtrzavapli.html

[R26] 命令替换
来源：http://hz.yuanzhike.top/gtghnwcpda.html

now=$(date +%F); echo "$now"
来源：http://hz.andypj.xyz/gtdiyhxoxr.html

[R27] 算术展开
来源：http://hz.zhengqikj.top/gtzmgmulmm.html

echo $((1 + 2 * 3))
来源：http://hz.pycfn.com/gtrkpauxkj.html

[R28] 浮点运算
来源：http://hz.hysaishi.cn/gtmiolgjti.html

echo "scale=2; 10/3" | bc
来源：http://hz.cashguo.top/gtotlixerz.html

[R29] 定义函数
来源：http://hz.xinyue.icu/gtsldvagsz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhaomingkeji.xyz/gttvpiewkn.html

[R30] 函数返回状态码
来源：http://hz.hammf.cn/gtvlawesqt.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xingfuxueyuan.xyz/gtfbruwvma.html

[R31] 局部变量
来源：http://hz.hammf.cn/gtwxvacfdk.html

f() { local x=1; echo "$x"; }
来源：http://hz.shanyushiyangtech.top/gtbiebhqhs.html

[R32] 参数个数校验
来源：http://hz.yj202588.top/gtatkgxrak.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yongpay.top/gtyhcoccvw.html

[R33] 捕获错误并提示行号
来源：http://hz.ydjk.org.cn/gtesvhulqf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.nanxinkj.top/gtfihdvyit.html

[R34] 退出时清理
来源：http://hz.cqqwz.cn/gtcmuvppfj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.kuanghao11.cn/gtgpdveeet.html

[R35] 后台执行并等待
来源：http://hz.tian-w.cn/gtcodxuolc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhengqikj.top/gtwlcmddnq.html

[R36] 并发执行多个任务
来源：http://hz.sufxvd.cn/gtwmurfjxx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.quarkkingdee.top/gtbcpzznkm.html

[R37] 把输出赋给变量
来源：http://hz.quarkkingdee.top/gtvrbiiszs.html

files=$(ls -1)
来源：http://hz.yj20258888.top/gtwrnuhwis.html

[R38] 管道串联
来源：http://hz.316326.xyz/gtknrmtvtm.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cucudq.cn/gtbhgsieal.html

[R39] 重定向标准输出与错误
来源：http://hz.chenzaomai.com/gtacfdnyap.html

cmd > out.log 2>&1
来源：http://hz.sweek.top/gtlhxajobx.html

[R40] 追加写日志
来源：http://hz.0kj1m.cn/gtvklyvvos.html

echo "log" >> out.log
来源：http://hz.ybcxt.top/gthfzyxqgx.html

[R41] 丢弃输出
来源：http://hz.jianghu66.top/gtfbphimnq.html

cmd >/dev/null 2>&1
来源：http://hz.zhaomingkeji.xyz/gtxlkvbsxl.html

[R42] 输入重定向
来源：http://hz.dianchejie.cn/gttzdxznkf.html

wc -l < a.txt
来源：http://hz.hysaishi.cn/gtybvjqqfy.html

[R43] 按名字查找文件
来源：http://hz.yangfankeji.com/gthzsouuii.html

find . -name "*.log" -type f
来源：http://hz.cheryme.top/gtwmzdaytw.html

[R44] 按修改时间查找
来源：http://hz.cqqwz.cn/gtnlplediv.html

find . -mtime -7 -type f
来源：http://hz.fengsongda.top/gtnvgfzhfe.html

[R45] 批量删除
来源：http://hz.yanxiufei.cn/gtuochzjyl.html

find . -name "*.tmp" -delete
来源：http://hz.kuanghao11.cn/gtcsuodqze.html

[R46] 递归替换文件内容
来源：http://hz.cdnleiting.top/gtjxfcvjta.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.aibaodan.cn/gthrqvroun.html

[R47] sed 单行替换
来源：http://hz.9152youxi.cn/gtcprrbipt.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ydzc1.top/gthxvyegff.html

[R48] awk 取指定列
来源：http://hz.9152youxi.cn/gthqbtjjtq.html

awk '{print $1, $3}' a.txt
来源：http://hz.guannengcc.top/gtusgjbzuf.html

[R49] awk 带条件
来源：http://hz.jlsjyb.cn/gtfjiaader.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ppjwa.cn/gtnhlstwlu.html

[R50] awk 求和
来源：http://hz.shzxlz.cn/gtaurghden.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jinqigufen.top/gtteorquej.html

[R51] 排序去重取前几
来源：http://hz.shanyushiyangtech.top/gtlpzmhnft.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xuetiantiany.cn/gthtwcwngh.html

[R52] 统计行数
来源：http://hz.gzhubu.top/gtcyhtqycj.html

wc -l a.txt
来源：http://hz.ydzc1.top/gtarzuigla.html

[R53] 查看文件头与实时尾
来源：http://hz.yj20258.top/gtrvgwswkx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.haohaochexian.top/gtkdtkzate.html

[R54] 比较两个文件
来源：http://hz.zycfv.cn/gtojydossp.html

diff a.txt b.txt
来源：http://hz.yonumen.top/gtzoiewvtu.html

[R55] 压缩与解压
来源：http://hz.cqqwz.cn/gtsjhrquxw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.vqdsnc.cn/gtazszqzxl.html

[R56] 远程拷贝
来源：http://hz.hysaishi.cn/gtakfdbdkj.html

scp file user@host:/path/
来源：http://hz.fengsongda.top/gtwoyzwpck.html

[R57] 远程执行命令
来源：http://hz.xylfe.cn/gtbxrztgzv.html

ssh user@host 'uptime'
来源：http://hz.zhaomingkeji.xyz/gtqcjamndi.html

[R58] 下载文件
来源：http://hz.hnxiangtu.top/gtijjtmsvf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hysaishi.cn/gtacptkbks.html

[R59] 发 POST JSON
来源：http://hz.daxiang520.top/gtinuvakhp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hysaishi.cn/gtkejopfcr.html

[R60] 只看 HTTP 状态码
来源：http://hz.wangdashe.top/gtmuixizfp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.andypj.xyz/gtjcwjdxin.html

[R61] 磁盘占用
来源：http://hz.yanxiufei.cn/gtovihjyfx.html

df -h;  du -sh *
来源：http://hz.jinyuanbaomall.cn/gtnciqieuz.html

[R62] 找最占空间的文件
来源：http://hz.haohaochexian.top/gtsmndlbyq.html

du -ah . | sort -rh | head -10
来源：http://hz.nanxuanxn.top/gtbxdyhata.html

[R63] 内存与进程
来源：http://hz.guannengcc.top/gtjlsvhwax.html

free -h;  ps aux | grep nginx
来源：http://hz.kuanghao11.cn/gtiaaayfiy.html

[R64] 结束进程
来源：http://hz.ybcxt.top/gtbiuimwtd.html

kill -9 $(pgrep -f app.py)
来源：http://hz.andypj.xyz/gtdzzwvson.html

[R65] 查看端口占用
来源：http://hz.svipenyu.cn/gtecotrfws.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zycfv.cn/gtjmyqwwjk.html

[R66] 定时任务
来源：http://hz.hywenlv.cn/gtrvpyxrjo.html

crontab -e;  crontab -l
来源：http://hz.cucudq.cn/gtvauskqon.html

[R67] 生成随机十六进制串
来源：http://hz.nwbrower.top/gtcsjmlbtk.html

openssl rand -hex 16
来源：http://hz.ydzc1.top/gtzjvtqcay.html

[R68] 计算文件校验值
来源：http://hz.sysykeji.top/gtxqfcfufl.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.bjfxy.top/gtpicxvcjm.html

[R69] 生成随机密码
来源：http://hz.nanxuanxn.top/gtqyfqrqgm.html

head -c 16 /dev/urandom | base64
来源：http://hz.gotoacloud.top/gtxiigtgmb.html

[R70] 时间戳与互转
来源：http://hz.smart0.xyz/gtlnpqqqcv.html

date +%s;  date -d @1700000000
来源：http://hz.zhijiandao.cn/gtoflbgrbk.html

[R71] 日期格式化
来源：http://hz.jinqigufen.top/gtdzluvqzf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ybcxt.top/gtjhyegpvs.html

[R72] 等待端口就绪
来源：http://hz.tianlin.xyz/gtedraltld.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cashguo.top/gtdhhekgip.html

[R73] 分割大日志
来源：http://hz.nwbrower.top/gtyrgcvmen.html

split -l 1000 big.log part_
来源：http://hz.zhengqikj.top/gtpxkthdjw.html

[R74] 批量重命名
来源：http://hz.xinyue.icu/gtzsztxuqi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hnxiangtu.top/gtpiolxkln.html

[R75] 导出环境变量
来源：http://hz.aibaodan.cn/gtxsaqlbpr.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ivvv.top/gtvxignfeo.html

[R76] 使用临时文件
来源：http://hz.vqdsnc.cn/gtuvnyzcyx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhongyouzk.top/gttsmqsbds.html

[R77] 读取用户输入
来源：http://hz.yuxming.cn/gtxbhmcjdf.html

read -rp "请输入: " ans
来源：http://hz.havefunace.top/gthuffrstp.html

[R78] 交互式菜单
来源：http://hz.ppjwa.cn/gtmjwqtpto.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.redwolf501.top/gtfhizkodo.html

[R79] 解析命令行选项
来源：http://hz.jqgfzy.top/gtztpcgcal.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yonumen.top/gtittbdqgn.html

[R80] 查看脚本执行耗时
来源：http://hz.jinqigufen.top/gthysgphby.html

time ./run.sh
来源：http://hz.316326.xyz/gtjzavtwcb.html

================================================================================
来源：http://hz.jqgufenzy.top/gtxcxynzkl.html

S. C / C++ 专题
来源：http://hz.birdmap.top/gtpofmqjrx.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtcghpuerb.html

[S01] C：Hello World
来源：http://hz.snrcjt.cn/gtkynrvtec.html

#include <stdio.h>
来源：http://hz.snrcjt.cn/gtctwoqqej.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.vqdsnc.cn/gtkmzdtwhh.html

[S02] C：变量与格式化输出
来源：http://hz.iojbl.cn/gtubwnrgct.html

int a = 10; printf("%d\n", a);
来源：http://hz.yj202588.top/gtvjgxhprq.html

[S03] C：读入整数
来源：http://hz.ydjk.org.cn/gtyfdgzwod.html

int x; scanf("%d", &x);
来源：http://hz.ydzc1.top/gtvtyzmlap.html

[S04] C：字符串复制
来源：http://hz.smart0.xyz/gtwgttwzyl.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.wangdashe.top/gtwyadjckp.html

[S05] C：字符串长度
来源：http://hz.xziqi.cn/gtpfjpdlxh.html

strlen(s)
来源：http://hz.dianchejie.cn/gtsieurflk.html

[S06] C：字符串比较
来源：http://hz.nwbrower.top/gtcqrlaxma.html

strcmp(a, b) == 0
来源：http://hz.c1oappe.top/gtahpmakso.html

[S07] C：数组遍历求和
来源：http://hz.fengsongda.top/gtewbnodnt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.316326.xyz/gtackswnrg.html

[S08] C：动态内存分配与释放
来源：http://hz.yuxming.cn/gtyxzvdgda.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shangyingyoupin.top/gtdgelrsxd.html

[S09] C：结构体定义与初始化
来源：http://hz.sxryk.cn/gtqxbdkgfl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.0kj1m.cn/gttvuayfmj.html

[S10] C：指针与解引用
来源：http://hz.gaohongyu789.top/gtwllclrfs.html

int *p = &a;  *p = 5;
来源：http://hz.ivvv.top/gtpflbuxhm.html

[S11] C：逐行读文件
来源：http://hz.yuanzhike.top/gtnzuqfxst.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jiagoushi.top/gtsepadczc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hammf.cn/gtobsemfmt.html

fclose(f);
来源：http://hz.kuanghao11.cn/gtttlvdoxk.html

[S12] C：写文件
来源：http://hz.jlsjyb.cn/gtfqekyntm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jqgfzy.top/gtskgnlkxt.html

[S13] C：宏定义
来源：http://hz.shanyushiyangkeji.top/gtqndjoumi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yj20258888.top/gtdinegqdx.html

[S14] C：枚举
来源：http://hz.yvedp.cn/gtfvsruhqs.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhoulong.xyz/gtrkyugalv.html

[S15] C：类型转换
来源：http://hz.jlsjyb.cn/gtldqjperm.html

(double) a / b
来源：http://hz.zhengqikj.top/gtrfwmfuql.html

[S16] C：位操作置位
来源：http://hz.ybcxt.top/gtpshsfirn.html

x |= (1 << 3);
来源：http://hz.xuanzx.com/gtnzhiftds.html

[S17] C：安全拼接字符串
来源：http://hz.ivvv.top/gtuibwidtr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.wangshuangyany.cn/gtrwiiqxlt.html

[S18] C：命令行参数
来源：http://hz.hongshengwenyu.top/gtjfwpeddo.html

int main(int argc, char **argv)
来源：http://hz.daria6918.cn/gtgwbrppaf.html

[S19] C：快速排序
来源：http://hz.gzhubu.top/gtisoxrdww.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.gogol.net.cn/gtrlrwaxbq.html

[S20] C：二分查找
来源：http://hz.zhixingplan.top/gtgmijcpai.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.gogol.net.cn/gtbdcuapym.html

[S21] C：字符类别判断
来源：http://hz.hfpthk.cn/gtpxngkfof.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jyoumei.cn/gtdfmkeymg.html

[S22] C：字符串转数字
来源：http://hz.pengpengdd.cyou/gtxxsamzfz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.havefunace.top/gtdhfkixfi.html

[S23] C：随机数
来源：http://hz.daxiang520.top/gtzgdmeiqi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhiwuduotai.top/gtqwqsgzxd.html

[S24] C：获取本地时间
来源：http://hz.shanyushiyangkeji.top/gtefskhxwq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hfpthk.cn/gtuxfcfdfz.html

[S25] C：内存拷贝
来源：http://hz.ywan-chungtsiang.top/gthheqpzmy.html

memcpy(dst, src, n);
来源：http://hz.tianlin.xyz/gtuvsbkeem.html

[S26] C：内存清零
来源：http://hz.sxryk.cn/gtnjiwoxvk.html

memset(a, 0, sizeof a);
来源：http://hz.yj202588.top/gtenmfklak.html

[S27] C：定义常量
来源：http://hz.gzhubu.top/gtpattojxx.html

const double PI = 3.14159;
来源：http://hz.xuanzx.com/gteiybkjoh.html

[S28] C：静态变量
来源：http://hz.zhaomingkeji.xyz/gtdrjppjgb.html

static int counter = 0;
来源：http://hz.hammf.cn/gtjmdcjejn.html

[S29] C：变参函数
来源：http://hz.zdqjudy.top/gttddpmqap.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yj20258888.top/gtoidqzrsk.html

[S30] C：头文件保护
来源：http://hz.jinghuilouyu.cn/gtfsldlrij.html

#ifndef X_H
来源：http://hz.yvedp.cn/gtbnwesfqe.html

#define X_H
来源：http://hz.shanyushiyangkeji.top/gtmrfeckbj.html

#endif
来源：http://hz.hywenlv.cn/gtbwwdukvj.html

[S31] C++：Hello World
来源：http://hz.cucudq.cn/gtdmaxuync.html

#include <iostream>
来源：http://hz.jyoumei.cn/gthldynntu.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.haohaochexian.top/gtywgnxfsz.html

[S32] C++：字符串
来源：http://hz.shangyingyoupin.top/gteoqtuvql.html

std::string s = "hi";  s += "!";
来源：http://hz.aibaodan.cn/gtxezxcsgj.html

[S33] C++：vector 增删
来源：http://hz.pengpengdd.cyou/gtdonvdnyb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yj20258888.top/gtucenewvm.html

[S34] C++：遍历 vector
来源：http://hz.zhongyouzk.top/gtdhyzqxcm.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jinyuanbaomall.cn/gtqttbsoun.html

[S35] C++：map
来源：http://hz.cucudq.cn/gtftwalukl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yvedp.cn/gtoatqpyvj.html

[S36] C++：unordered_map
来源：http://hz.zhongyouzk.top/gtmecrbkui.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yonumen.top/gtnacgqfpd.html


<!-- 参考信息 -->