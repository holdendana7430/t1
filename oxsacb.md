代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.sufxvd.cn/gthepulezg.html

[Q60] 取上一行 / 下一行
来源：http://hz.sxryk.cn/gtzzublufd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.gogol.net.cn/gtotzvpepw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtqiridzls.html

[Q61] 移动平均
来源：http://hz.jianghu66.top/gtywlpmhqm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jiagoushi.top/gtnzsmbwdn.html

[Q62] 分组占比
来源：http://hz.hammf.cn/gtjmbygjzi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hfpthk.cn/gtrofbbnay.html

[Q63] 开启事务
来源：http://hz.0kj1m.cn/gthrlgbfla.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.meibo888.top/gtwvhjoffe.html

[Q64] 提交事务
来源：http://hz.nanxuanxn.top/gtufxwmifb.html

COMMIT;
来源：http://hz.havefunace.top/gtfmvbokty.html

[Q65] 回滚事务
来源：http://hz.yj202588.top/gtyqjyiqca.html

ROLLBACK;
来源：http://hz.snrcjt.cn/gtorooggbr.html

[Q66] 行锁查询
来源：http://hz.jiagoushi.top/gtcezotwvf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.andypj.xyz/gtbvhodkca.html

[Q67] 设置隔离级别
来源：http://hz.cdnleiting.top/gtyoidwujz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ywan-chungtsiang.top/gtmlhqxwrz.html

[Q68] 保存点
来源：http://hz.hfpthk.cn/gtlodghoex.html

SAVEPOINT sp1;
来源：http://hz.0kj1m.cn/gtpvmnbdaq.html

ROLLBACK TO sp1;
来源：http://hz.ybcxt.top/gttwyamfsw.html

[Q69] 查看执行计划
来源：http://hz.dianchejie.cn/gtbcnkslce.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ivvv.top/gtzljlqfij.html

[Q70] 更新统计信息
来源：http://hz.yuanzhike.top/gtstdttffl.html

ANALYZE TABLE users;
来源：http://hz.yongpay.top/gttqnlizwv.html

[Q71] 查看建表语句
来源：http://hz.vqdsnc.cn/gtrbcbsyrn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.kuanghao11.cn/gtnrjkeunz.html

[Q72] 查看索引
来源：http://hz.yueranfly.top/gtvhvyudqo.html

SHOW INDEX FROM users;
来源：http://hz.nanxuanxn.top/gtdfylrkqc.html

[Q73] 查看表状态
来源：http://hz.cucudq.cn/gtubxezukl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hysaishi.cn/gtzleesckb.html

[Q74] 强制使用索引
来源：http://hz.zhaomingkeji.xyz/gtdgjkcrbv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ehwqpu.com/gtmqhmbdrj.html

[Q75] 日期格式化
来源：http://hz.quarkkingdee.top/gtdbmciedx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhongyouzk.top/gtmdabhgsc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhoulong.xyz/gtnirjzfum.html

[Q76] 按天统计
来源：http://hz.kuanghao11.cn/gtvyyasxsd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ivvv.top/gtccptorlq.html

[Q77] 时间加减
来源：http://hz.hysaishi.cn/gtmbuzscpu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.daria6918.cn/gtfiwpcqku.html

[Q78] 当前时间
来源：http://hz.haohaochexian.top/gtrhblbtji.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.quarkkingdee.top/gtuawufaks.html

[Q79] 字符串拼接
来源：http://hz.jlsjyb.cn/gtruhvsjso.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhiwuduotai.top/gtouwcngwm.html

[Q80] 字符串截取
来源：http://hz.nanxuanxn.top/gtpkoagoxq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ydzc1.top/gtwrpewxzm.html

[Q81] 字符串替换
来源：http://hz.fengsongda.top/gtgegrbfrf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shuidangran.top/gtydvxxijr.html

[Q82] 字符长度与字节长度
来源：http://hz.fzhhl.top/gtgldkzoxw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.0kj1m.cn/gtrrpurzqc.html

[Q83] 大小写转换
来源：http://hz.nwbrower.top/gtkspkocqk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhoulong.xyz/gtunmulsak.html

[Q84] 去除首尾空格
来源：http://hz.yanxiufei.cn/gtcjcjxxen.html

SELECT TRIM(name) FROM users;
来源：http://hz.dianchejie.cn/gtixozuaps.html

[Q85] 数值取整
来源：http://hz.zycfv.cn/gtvwnftrab.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ywan-chungtsiang.top/gthkfomghx.html

[Q86] 读取 JSON 字段
来源：http://hz.aibaodan.cn/gtttrjkzeh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.smart0.xyz/gtacbcfzwb.html

[Q87] JSON 字段做条件
来源：http://hz.fzhhl.top/gtppwquycb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.gotoacloud.top/gtztatamzl.html

[Q88] 行转列（条件聚合）
来源：http://hz.zdqjudy.top/gtwylojget.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.feifeiyinyue.top/gtiatvbcum.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xuanzx.com/gtiijzoibx.html

[Q89] 判断表是否存在
来源：http://hz.hammf.cn/gtimuqigzv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yuxming.cn/gtfkrihnky.html

[Q90] 生成序号列
来源：http://hz.cqqwz.cn/gtrtphvexs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.havefunace.top/gtbwnsoxqq.html

================================================================================
来源：http://hz.c1oappe.top/gtgssgiyki.html

R. Bash 专题
来源：http://hz.yj20258888.top/gtxmuqswda.html

================================================================================
来源：http://hz.nanxinkj.top/gtmorukayx.html

[R01] shebang 与严格模式
来源：http://hz.meibo888.top/gtirvfrltq.html

#!/usr/bin/env bash
来源：http://hz.yj20258.top/gtmmhpbvjb.html

set -euo pipefail
来源：http://hz.birdmap.top/gtbcxnsgvy.html

[R02] 变量赋值与使用
来源：http://hz.mhx1999.top/gtyenikcld.html

name="Tom"; echo "$name"
来源：http://hz.jinyuanbaomall.cn/gtdyjftmku.html

[R03] 只读变量
来源：http://hz.hnxiangtu.top/gttjngnncb.html

readonly PI=3.14
来源：http://hz.shanyushiyangkeji.top/gtgnxsumdc.html

[R04] 位置参数
来源：http://hz.shuidangran.top/gtviigrvsj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.sweek.top/gtgcjzadei.html

[R05] 参数默认值
来源：http://hz.feifeiyinyue.top/gtcnbidpss.html

name="${1:-default}"
来源：http://hz.havefunace.top/gtulybzfya.html

[R06] 判断命令是否存在
来源：http://hz.iojbl.cn/gtkdlaspdm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinghuilouyu.cn/gtqifhdknw.html

[R07] if 判断文件
来源：http://hz.wangshuangyany.cn/gtexmkdpud.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.gaohongyu789.top/gtvvhkeojt.html

[R08] 数值比较
来源：http://hz.nanxuanxn.top/gtlgxpvtmh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.mhx1999.top/gterbgtrlz.html

[R09] 字符串比较
来源：http://hz.meibo888.top/gteasllxer.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ydzc1.top/gtbrcyihyq.html

[R10] 正则匹配
来源：http://hz.zhaomingkeji.xyz/gtihquwltd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.svipenyu.cn/gtpqdvuwdc.html

[R11] case 多分支
来源：http://hz.dashuyun.cn/gtnyekchlq.html

case "$1" in
来源：http://hz.ydzc1.top/gtkmnrxlvb.html

start) echo "启动" ;;
来源：http://hz.zdqjudy.top/gttamyjtyy.html

stop)  echo "停止" ;;
来源：http://hz.aizwys.cn/gtaqbavvxh.html

*)     echo "未知命令" ;;
来源：http://hz.ybcxt.top/gtepixaxnx.html

esac
来源：http://hz.yj202588.top/gtxamiommt.html

[R12] for 遍历文件
来源：http://hz.shanyushiyangkeji.top/gtsfwavqsd.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jianghu66.top/gtvopqclov.html

[R13] for 计数循环
来源：http://hz.sweek.top/gtbipmqatf.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zycfv.cn/gticnhjegh.html

[R14] C 风格 for
来源：http://hz.bjfxy.top/gtjfhrcuaa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.dashuyun.cn/gtvqkxjxkc.html

[R15] while 逐行读文件
来源：http://hz.ybcxt.top/gtlkusnckm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.quarkkingdee.top/gtgsrldfgh.html

[R16] until 等待条件
来源：http://hz.nanxuanxn.top/gtldumhush.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.nwbrower.top/gtueurfids.html

[R17] 数组定义与取值
来源：http://hz.sxryk.cn/gtngvxrjfb.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.svipenyu.cn/gtqnzdgrxl.html

[R18] 遍历数组
来源：http://hz.birdmap.top/gtbhxalrcz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yuxming.cn/gtbrxntedr.html

[R19] 数组长度
来源：http://hz.xuetiantiany.cn/gtjbqwardd.html

echo "${#arr[@]}"
来源：http://hz.svipenyu.cn/gtamovjghy.html

[R20] 关联数组（字典）
来源：http://hz.zhixingplan.top/gtkpkicxxd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yuxming.cn/gtgpskniuw.html

[R21] 字符串长度
来源：http://hz.fengsongda.top/gtlkbdogsh.html

echo "${#s}"
来源：http://hz.wangdashe.top/gteclwbfzw.html

[R22] 截取子串
来源：http://hz.yanxiufei.cn/gtfcpznxvg.html

echo "${s:0:5}"
来源：http://hz.xuetiantiany.cn/gtnpuhphtx.html

[R23] 字符串替换
来源：http://hz.zhaomingkeji.xyz/gtvllrsmzu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.dianchejie.cn/gtxeymykbm.html

[R24] 大小写转换
来源：http://hz.tian-w.cn/gtrzbksmvg.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ywan-chungtsiang.top/gtjuarwcir.html

[R25] 去后缀 / 去前缀
来源：http://hz.guowangkeji.top/gtyeytpxcn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shzxlz.cn/gtofjiasrq.html

[R26] 命令替换
来源：http://hz.ydjk.org.cn/gtxprumyyu.html

now=$(date +%F); echo "$now"
来源：http://hz.zycfv.cn/gtzsvzmqax.html

[R27] 算术展开
来源：http://hz.chenjidiqi.icu/gtxgnhdxov.html

echo $((1 + 2 * 3))
来源：http://hz.daria6918.cn/gtuyyfclju.html

[R28] 浮点运算
来源：http://hz.feifeiyinyue.top/gtoofrusnh.html

echo "scale=2; 10/3" | bc
来源：http://hz.xuetiantiany.cn/gtqzkkoaaz.html

[R29] 定义函数
来源：http://hz.xuanzx.com/gtcsohwjwd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.svipenyu.cn/gtscmttuuk.html

[R30] 函数返回状态码
来源：http://hz.tanke756.top/gthtsdlstj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.fzhhl.top/gtjtkcqjjk.html

[R31] 局部变量
来源：http://hz.meibo888.top/gtsjegdhoy.html

f() { local x=1; echo "$x"; }
来源：http://hz.wangshuangyany.cn/gtgtpsetzx.html

[R32] 参数个数校验
来源：http://hz.nanxuanxn.top/gtwtbuhzol.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hammf.cn/gtufcudklr.html

[R33] 捕获错误并提示行号
来源：http://hz.hnqzz.top/gttzbdpkjl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.9152youxi.cn/gtqdcnsrhl.html

[R34] 退出时清理
来源：http://hz.jqgufenzy.top/gtugyhpzta.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.shanyushiyangtech.top/gtmtbyhlys.html

[R35] 后台执行并等待
来源：http://hz.yvedp.cn/gtrsehxrun.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhengqikj.top/gtpvshvzey.html

[R36] 并发执行多个任务
来源：http://hz.xylfe.cn/gtmfuvjlco.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yuxming.cn/gtheplfiio.html

[R37] 把输出赋给变量
来源：http://hz.yueranfly.top/gtlqfosxjt.html

files=$(ls -1)
来源：http://hz.zhixingplan.top/gtsoqsieic.html

[R38] 管道串联
来源：http://hz.yvedp.cn/gttgpfhcnr.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yj20258888.top/gtxceplqwv.html

[R39] 重定向标准输出与错误
来源：http://hz.hysaishi.cn/gtbucrqgbc.html

cmd > out.log 2>&1
来源：http://hz.gzhubu.top/gttutnbjgz.html

[R40] 追加写日志
来源：http://hz.feifeiyinyue.top/gtvwtudgio.html

echo "log" >> out.log
来源：http://hz.zhaomingkeji.xyz/gtistrfwov.html

[R41] 丢弃输出
来源：http://hz.nanxinkj.top/gtifmnqtbv.html

cmd >/dev/null 2>&1
来源：http://hz.yongpay.top/gtcaggnizu.html

[R42] 输入重定向
来源：http://hz.chenjidiqi.icu/gtvjneexcb.html

wc -l < a.txt
来源：http://hz.snrcjt.cn/gtcygxqwoo.html

[R43] 按名字查找文件
来源：http://hz.jqgufenzy.top/gterssdtvm.html

find . -name "*.log" -type f
来源：http://hz.daxiang520.top/gturvdjxcn.html

[R44] 按修改时间查找
来源：http://hz.jlsjyb.cn/gtluzxmmrg.html

find . -mtime -7 -type f
来源：http://hz.smart0.xyz/gtwddjywwf.html

[R45] 批量删除
来源：http://hz.0kj1m.cn/gtjwpmpwbw.html

find . -name "*.tmp" -delete
来源：http://hz.jyoumei.cn/gtsbtgkdhy.html

[R46] 递归替换文件内容
来源：http://hz.fzhhl.top/gtyctpxmgh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.feifeiyinyue.top/gtqpicdjpm.html

[R47] sed 单行替换
来源：http://hz.yj20258888.top/gtldxxemkr.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.vqdsnc.cn/gtvzyvgxte.html

[R48] awk 取指定列
来源：http://hz.sysykeji.top/gtkswzxgsh.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhijiandao.cn/gtezjcyvwt.html

[R49] awk 带条件
来源：http://hz.ywan-chungtsiang.top/gtjdioisne.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hysaishi.cn/gtkeyyrema.html

[R50] awk 求和
来源：http://hz.birdmap.top/gtjyptgcfn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.wangshuangyany.cn/gtuvlycbpq.html

[R51] 排序去重取前几
来源：http://hz.yongpay.top/gtnmzrslnq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zycfv.cn/gtkbkwwtre.html

[R52] 统计行数
来源：http://hz.ywan-chungtsiang.top/gthkarsefc.html

wc -l a.txt
来源：http://hz.sxryk.cn/gtutsxncru.html

[R53] 查看文件头与实时尾
来源：http://hz.xingfuxueyuan.xyz/gtuewcqxtj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.smart0.xyz/gtpqsfmpfy.html

[R54] 比较两个文件
来源：http://hz.pengpengdd.cyou/gtfapmzoiz.html

diff a.txt b.txt
来源：http://hz.pycfn.com/gtgngwvscj.html

[R55] 压缩与解压
来源：http://hz.daxiang520.top/gthmwbhoft.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.quarkkingdee.top/gtwqkfgbhg.html

[R56] 远程拷贝
来源：http://hz.ydzc1.top/gttvfwjxvq.html

scp file user@host:/path/
来源：http://hz.yj20258888.top/gtusobxtzh.html

[R57] 远程执行命令
来源：http://hz.nwbrower.top/gtmtympkfg.html

ssh user@host 'uptime'
来源：http://hz.xziqi.cn/gttwusfirp.html

[R58] 下载文件
来源：http://hz.shangyingyoupin.top/gtjnmhanyt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ppjwa.cn/gtorzvezyb.html

[R59] 发 POST JSON
来源：http://hz.meibo888.top/gtfedqykci.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhijiandao.cn/gtkmetothb.html

[R60] 只看 HTTP 状态码
来源：http://hz.gaohongyu789.top/gtfevbgosp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jiagoushi.top/gtrisvgdom.html

[R61] 磁盘占用
来源：http://hz.pengpengdd.cyou/gtkhqarpll.html

df -h;  du -sh *
来源：http://hz.mhx1999.top/gtwvotvfqa.html

[R62] 找最占空间的文件
来源：http://hz.c1oappe.top/gtqdldsgeo.html

du -ah . | sort -rh | head -10
来源：http://hz.wangdashe.top/gtevllwsza.html

[R63] 内存与进程
来源：http://hz.zhijiandao.cn/gtmewzdscj.html

free -h;  ps aux | grep nginx
来源：http://hz.snrcjt.cn/gtkqrbtvbv.html

[R64] 结束进程
来源：http://hz.xziqi.cn/gtctqmmhuj.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jqgfzy.top/gtoitdgaog.html

[R65] 查看端口占用
来源：http://hz.haohaochexian.top/gtkymgvgtl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.sweek.top/gtpcdllgur.html

[R66] 定时任务
来源：http://hz.c1oappe.top/gtvjhfcqpm.html

crontab -e;  crontab -l
来源：http://hz.pycfn.com/gtapjmctnt.html

[R67] 生成随机十六进制串
来源：http://hz.shuidangran.top/gtzwppsccq.html

openssl rand -hex 16
来源：http://hz.gotoacloud.top/gtvfdzfjee.html

[R68] 计算文件校验值
来源：http://hz.tianlin.xyz/gtrpdiytiv.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shanyushiyangtech.top/gtejydknmr.html

[R69] 生成随机密码
来源：http://hz.chenlongwang.top/gtuwgtaqmm.html

head -c 16 /dev/urandom | base64
来源：http://hz.tian-w.cn/gteaszoeui.html

[R70] 时间戳与互转
来源：http://hz.mhx1999.top/gtvocihfye.html

date +%s;  date -d @1700000000
来源：http://hz.wangdashe.top/gteqdxhoom.html

[R71] 日期格式化
来源：http://hz.andypj.xyz/gtoglzijmm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.tian-w.cn/gtpjtbmutd.html

[R72] 等待端口就绪
来源：http://hz.0kj1m.cn/gtvgshgpqt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hammf.cn/gteqxgomyo.html

[R73] 分割大日志
来源：http://hz.hywenlv.cn/gtyndfyryk.html

split -l 1000 big.log part_
来源：http://hz.jianghu66.top/gtzugtasta.html

[R74] 批量重命名
来源：http://hz.smart0.xyz/gtudhwmtak.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.andypj.xyz/gtqbvzavqe.html

[R75] 导出环境变量
来源：http://hz.ehwqpu.com/gtpfemzhcg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.gaohongyu789.top/gtuwmdhoqt.html

[R76] 使用临时文件
来源：http://hz.0kj1m.cn/gtfgwetpmn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.birdmap.top/gtjidodogr.html

[R77] 读取用户输入
来源：http://hz.feifeiyinyue.top/gtnfayhirk.html

read -rp "请输入: " ans
来源：http://hz.quarkkingdee.top/gtkikdwdvo.html

[R78] 交互式菜单
来源：http://hz.dashuyun.cn/gtgayoiqxu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.vqdsnc.cn/gttmetcgqj.html

[R79] 解析命令行选项
来源：http://hz.cucudq.cn/gtptmvoggg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.chenjidiqi.icu/gtnnzfdtai.html

[R80] 查看脚本执行耗时
来源：http://hz.daxiang520.top/gtnpemgwzs.html

time ./run.sh
来源：http://hz.ywan-chungtsiang.top/gtdwvkvlne.html

================================================================================
来源：http://hz.yongpay.top/gtuakyvfzh.html

S. C / C++ 专题
来源：http://hz.shanyushiyangtech.top/gtmzazmndn.html

================================================================================
来源：http://hz.nwbrower.top/gtyztqzwkg.html

[S01] C：Hello World
来源：http://hz.pycfn.com/gthkrjvedv.html

#include <stdio.h>
来源：http://hz.zhoulong.xyz/gtfvqftroj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.aibaodan.cn/gtxiwwzuuz.html

[S02] C：变量与格式化输出
来源：http://hz.meibo888.top/gtdztzfqzg.html

int a = 10; printf("%d\n", a);
来源：http://hz.shuidangran.top/gtupwtcvtv.html

[S03] C：读入整数
来源：http://hz.shanyushiyangtech.top/gtgnqxjubw.html

int x; scanf("%d", &x);
来源：http://hz.redwolf501.top/gtwmmjpaqf.html

[S04] C：字符串复制
来源：http://hz.cucudq.cn/gtaxdfeyhm.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yonumen.top/gtwowiedgx.html

[S05] C：字符串长度
来源：http://hz.dashuyun.cn/gtqkfkjspb.html

strlen(s)
来源：http://hz.hysaishi.cn/gtwufrxagx.html

[S06] C：字符串比较
来源：http://hz.yueranfly.top/gtbjypszkt.html

strcmp(a, b) == 0
来源：http://hz.sxryk.cn/gthluxvavj.html

[S07] C：数组遍历求和
来源：http://hz.ppjwa.cn/gtirvdoixc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.c1oappe.top/gtzmmhtgzb.html

[S08] C：动态内存分配与释放
来源：http://hz.mhx1999.top/gtlinmkgyz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.nanxuanxn.top/gtlspsuwvh.html

[S09] C：结构体定义与初始化
来源：http://hz.ehwqpu.com/gthufzkkeu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.iojbl.cn/gttmvupgif.html

[S10] C：指针与解引用
来源：http://hz.yongpay.top/gtmqahlbzs.html

int *p = &a;  *p = 5;
来源：http://hz.chenlongwang.top/gttuqmzblo.html

[S11] C：逐行读文件
来源：http://hz.dashuyun.cn/gtadedthjv.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sweek.top/gtkrmpdlvn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.aizwys.cn/gtfdjcmstb.html

fclose(f);
来源：http://hz.pengpengdd.cyou/gttpiszjbm.html

[S12] C：写文件
来源：http://hz.daria6918.cn/gtuvajgbdk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ydjk.org.cn/gtendqbuyy.html

[S13] C：宏定义
来源：http://hz.guowangkeji.top/gtatcwnnbc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yanxiufei.cn/gtupyufowp.html

[S14] C：枚举
来源：http://hz.yueranfly.top/gtnwugxsjw.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.shanyushiyangtech.top/gtdxmmhimx.html

[S15] C：类型转换
来源：http://hz.jinqigfzy.top/gtevuhvvez.html

(double) a / b
来源：http://hz.cqqwz.cn/gtfpwcarmz.html

[S16] C：位操作置位
来源：http://hz.nanxinkj.top/gtuallwbjl.html

x |= (1 << 3);
来源：http://hz.nanxuanxn.top/gtizykdbey.html

[S17] C：安全拼接字符串
来源：http://hz.yj20258.top/gtowqtavhm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.vqdsnc.cn/gtrllfaeba.html

[S18] C：命令行参数
来源：http://hz.chenjidiqi.icu/gtksegdrvq.html

int main(int argc, char **argv)
来源：http://hz.redwolf501.top/gtnaezbavt.html

[S19] C：快速排序
来源：http://hz.xuanzx.com/gtactpqhih.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.316326.xyz/gtkwitypgg.html

[S20] C：二分查找
来源：http://hz.ydjk.org.cn/gtkxlmafnw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yuanzhike.top/gtlniafzze.html

[S21] C：字符类别判断
来源：http://hz.ydzc1.top/gtumowuphp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhoulong.xyz/gtprmryepu.html

[S22] C：字符串转数字
来源：http://hz.gotoacloud.top/gtftscrvcc.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.guannengcc.top/gtjxpkxipj.html

[S23] C：随机数
来源：http://hz.guowangkeji.top/gtdunjulph.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhiwuduotai.top/gtznarmwod.html

[S24] C：获取本地时间
来源：http://hz.jqgufenzy.top/gtfguuclrn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.daria6918.cn/gtrjnvlksl.html

[S25] C：内存拷贝
来源：http://hz.yuanzhike.top/gtzlhsvpaz.html

memcpy(dst, src, n);
来源：http://hz.sweek.top/gtklkfytzb.html

[S26] C：内存清零
来源：http://hz.cheryme.top/gtqinpwucg.html

memset(a, 0, sizeof a);
来源：http://hz.quarkkingdee.top/gtgrzfokbt.html

[S27] C：定义常量
来源：http://hz.jinqigufen.top/gtmfvztsgb.html

const double PI = 3.14159;
来源：http://hz.zhengqikj.top/gtqxwusihv.html

[S28] C：静态变量
来源：http://hz.pengpengdd.cyou/gtlvmlxmgn.html

static int counter = 0;
来源：http://hz.smart0.xyz/gtddghdxfa.html

[S29] C：变参函数
来源：http://hz.zhongyouzk.top/gtcsywmapr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.tanke756.top/gtoasaxmjy.html

[S30] C：头文件保护
来源：http://hz.jianghu66.top/gtivttibkr.html


<!-- 参考信息 -->