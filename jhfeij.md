代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.dashuyun.cn/gtastqkgdu.html

[Q52] 删除指定行
来源：http://hz.ppjwa.cn/gtwgulcrgu.html

DELETE FROM users WHERE id = 10;
来源：http://hz.shanyushiyangkeji.top/gtcaxrzkga.html

[Q53] 按条件删除
来源：http://hz.yj20258.top/gtcbbvozwz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.birdmap.top/gtmuruwmmy.html

[Q54] 清空表
来源：http://hz.tianlin.xyz/gtklwyrrmv.html

TRUNCATE TABLE logs;
来源：http://hz.hammf.cn/gtgzfngcou.html

[Q55] 排名（并列占位）
来源：http://hz.guowangkeji.top/gthujypbnc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yueranfly.top/gtpxkymmom.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhengqikj.top/gtrnprzzmi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ehwqpu.com/gtwfuwqath.html

[Q57] 行号
来源：http://hz.hfpthk.cn/gtyjwkmova.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtabdgfyay.html

[Q58] 累计求和
来源：http://hz.sxryk.cn/gtedazotba.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ydjk.org.cn/gtvbfbqakx.html

[Q59] 分组内累计
来源：http://hz.guowangkeji.top/gtjwaklcmz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.gzhubu.top/gtihyhjulk.html

[Q60] 取上一行 / 下一行
来源：http://hz.nanxuanxn.top/gtkvtzgcan.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.vqdsnc.cn/gtendifabc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.daria6918.cn/gtbpyxlrhi.html

[Q61] 移动平均
来源：http://hz.jqgufenzy.top/gtqxkpzdis.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.pycfn.com/gtinhwwyty.html

[Q62] 分组占比
来源：http://hz.hysaishi.cn/gtbjkmcudm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ywan-chungtsiang.top/gtbbarfdtg.html

[Q63] 开启事务
来源：http://hz.wangdashe.top/gtpcfnzzoi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.kuanghao11.cn/gttzlxgzic.html

[Q64] 提交事务
来源：http://hz.cdnleiting.top/gtmrzklchr.html

COMMIT;
来源：http://hz.quarkkingdee.top/gtjtejdzte.html

[Q65] 回滚事务
来源：http://hz.cqqwz.cn/gtjvotfzxl.html

ROLLBACK;
来源：http://hz.0kj1m.cn/gtqoidcbec.html

[Q66] 行锁查询
来源：http://hz.zdqjudy.top/gtvxztzpbe.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.dianchejie.cn/gtvdjfrgxr.html

[Q67] 设置隔离级别
来源：http://hz.dashuyun.cn/gtilvyftku.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cqqwz.cn/gtfajfhfni.html

[Q68] 保存点
来源：http://hz.svipenyu.cn/gtkbbesymt.html

SAVEPOINT sp1;
来源：http://hz.yonumen.top/gtzbtenlxx.html

ROLLBACK TO sp1;
来源：http://hz.jinghuilouyu.cn/gtdzmyemtf.html

[Q69] 查看执行计划
来源：http://hz.smart0.xyz/gtlkysjygm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.shanyushiyangtech.top/gtxxwdlloj.html

[Q70] 更新统计信息
来源：http://hz.zhiwuduotai.top/gtkzmrmlsk.html

ANALYZE TABLE users;
来源：http://hz.cqqwz.cn/gtlzwkewso.html

[Q71] 查看建表语句
来源：http://hz.sufxvd.cn/gtnahwnlgs.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hywenlv.cn/gtscnmnukx.html

[Q72] 查看索引
来源：http://hz.tanke756.top/gtaphcmwvl.html

SHOW INDEX FROM users;
来源：http://hz.jqgufenzy.top/gtytwyjyyu.html

[Q73] 查看表状态
来源：http://hz.havefunace.top/gticsdgolq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.aibaodan.cn/gtsfgfguze.html

[Q74] 强制使用索引
来源：http://hz.pycfn.com/gtwcwyvouj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ydzc1.top/gtzhtlfpnx.html

[Q75] 日期格式化
来源：http://hz.aizwys.cn/gtvnbfelwc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.tanke756.top/gtyebollus.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zycfv.cn/gtnsnmhdgp.html

[Q76] 按天统计
来源：http://hz.nwbrower.top/gtzwucclyc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.9152youxi.cn/gthrkgmyhb.html

[Q77] 时间加减
来源：http://hz.sufxvd.cn/gtphaxycui.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.pengpengdd.cyou/gtrhuqbxoi.html

[Q78] 当前时间
来源：http://hz.vqdsnc.cn/gtvycmtkjj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yongpay.top/gtzjdgshja.html

[Q79] 字符串拼接
来源：http://hz.hnxiangtu.top/gtfvkpgwsj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cashguo.top/gtlpktqahc.html

[Q80] 字符串截取
来源：http://hz.yangfankeji.com/gtqzzbliov.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zdqjudy.top/gtbnaxhkhl.html

[Q81] 字符串替换
来源：http://hz.ybcxt.top/gtndknkobf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.svipenyu.cn/gtuhbowsxg.html

[Q82] 字符长度与字节长度
来源：http://hz.xziqi.cn/gtsydoxifv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.tian-w.cn/gtzjehwpfu.html

[Q83] 大小写转换
来源：http://hz.daxiang520.top/gtxvznmeou.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hnqzz.top/gtcuueptid.html

[Q84] 去除首尾空格
来源：http://hz.hammf.cn/gtxqjfjcck.html

SELECT TRIM(name) FROM users;
来源：http://hz.zdqjudy.top/gtxwgnmbao.html

[Q85] 数值取整
来源：http://hz.fzhhl.top/gtremtdqaz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.andypj.xyz/gtdkqvexlz.html

[Q86] 读取 JSON 字段
来源：http://hz.xuetiantiany.cn/gtcthmjviq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xuanzx.com/gtjacuwngq.html

[Q87] JSON 字段做条件
来源：http://hz.hammf.cn/gttimwgjzn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yongpay.top/gtwkjydbit.html

[Q88] 行转列（条件聚合）
来源：http://hz.c1oappe.top/gtnebswwir.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jianghu66.top/gtgneumnxb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hongshengwenyu.top/gtdpccrbsq.html

[Q89] 判断表是否存在
来源：http://hz.jqgufenzy.top/gtqjwvrkdt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.mhx1999.top/gtrcypkuah.html

[Q90] 生成序号列
来源：http://hz.meibo888.top/gtlcnucdox.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.bjfxy.top/gtvcgeqvwg.html

================================================================================
来源：http://hz.svipenyu.cn/gtisrriuld.html

R. Bash 专题
来源：http://hz.vqdsnc.cn/gtrxorfxfm.html

================================================================================
来源：http://hz.cucudq.cn/gtythiektf.html

[R01] shebang 与严格模式
来源：http://hz.fzhhl.top/gtxzgctvid.html

#!/usr/bin/env bash
来源：http://hz.0kj1m.cn/gtwqjcjdxx.html

set -euo pipefail
来源：http://hz.ybcxt.top/gtisgdwikk.html

[R02] 变量赋值与使用
来源：http://hz.zhaomingkeji.xyz/gtjkmsrsmb.html

name="Tom"; echo "$name"
来源：http://hz.gaohongyu789.top/gtndvyegfw.html

[R03] 只读变量
来源：http://hz.xingfuxueyuan.xyz/gtxqzovptq.html

readonly PI=3.14
来源：http://hz.hysaishi.cn/gtjmnlqzvi.html

[R04] 位置参数
来源：http://hz.tian-w.cn/gtuiuzuiwe.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.haohaochexian.top/gtxirdkfii.html

[R05] 参数默认值
来源：http://hz.pycfn.com/gtdrzfblvf.html

name="${1:-default}"
来源：http://hz.chenlongwang.top/gttnxiqigr.html

[R06] 判断命令是否存在
来源：http://hz.ywan-chungtsiang.top/gtbvdsafec.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.tianlin.xyz/gtxrakjqny.html

[R07] if 判断文件
来源：http://hz.xziqi.cn/gtvjfoydcp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.fengsongda.top/gtfefjkjyh.html

[R08] 数值比较
来源：http://hz.zhijiandao.cn/gtxmoideyi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jiagoushi.top/gtdeapcbkz.html

[R09] 字符串比较
来源：http://hz.birdmap.top/gtpjuowvnn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.cqqwz.cn/gtqljybbbp.html

[R10] 正则匹配
来源：http://hz.bjfxy.top/gtjguyhxjb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.fengsongda.top/gtoghmkoaq.html

[R11] case 多分支
来源：http://hz.cdnleiting.top/gtogmliopq.html

case "$1" in
来源：http://hz.zhixingplan.top/gtgawiuggk.html

start) echo "启动" ;;
来源：http://hz.aibaodan.cn/gtkbrhwkjh.html

stop)  echo "停止" ;;
来源：http://hz.shuidangran.top/gtjmmqdvne.html

*)     echo "未知命令" ;;
来源：http://hz.daria6918.cn/gtiupiyjzy.html

esac
来源：http://hz.jinqigfzy.top/gtqwmtoxno.html

[R12] for 遍历文件
来源：http://hz.jiagoushi.top/gtmpqexmyi.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yuanzhike.top/gtijunjega.html

[R13] for 计数循环
来源：http://hz.nanxuanxn.top/gtfcapmjjm.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shanyushiyangkeji.top/gtyzjvbhsx.html

[R14] C 风格 for
来源：http://hz.nwbrower.top/gtteapqlwj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jinqigufen.top/gtjmnsyvgf.html

[R15] while 逐行读文件
来源：http://hz.yj202588.top/gtlgbdmqxx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.gaohongyu789.top/gtmwfqcivt.html

[R16] until 等待条件
来源：http://hz.sweek.top/gtjbavoucm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shanyushiyangtech.top/gtaoyukzvr.html

[R17] 数组定义与取值
来源：http://hz.ppjwa.cn/gtmhsqwjph.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xuetiantiany.cn/gtiacagnbi.html

[R18] 遍历数组
来源：http://hz.jinqigfzy.top/gtmxprsfoo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.guannengcc.top/gtmkrgitox.html

[R19] 数组长度
来源：http://hz.yueranfly.top/gtpyolhife.html

echo "${#arr[@]}"
来源：http://hz.jqgfzy.top/gtaqxstdsj.html

[R20] 关联数组（字典）
来源：http://hz.zdqjudy.top/gtizsfwetm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xylfe.cn/gtkiyzpltw.html

[R21] 字符串长度
来源：http://hz.xinyue.icu/gtidxdvsly.html

echo "${#s}"
来源：http://hz.cashguo.top/gtdiybzrgg.html

[R22] 截取子串
来源：http://hz.iojbl.cn/gtryaxdkit.html

echo "${s:0:5}"
来源：http://hz.yonumen.top/gtebiosyso.html

[R23] 字符串替换
来源：http://hz.zhixingplan.top/gtkwhbwvvv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhiwuduotai.top/gtcycdgkkn.html

[R24] 大小写转换
来源：http://hz.jqgufenzy.top/gtzgtronts.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.daria6918.cn/gtnzjwngvw.html

[R25] 去后缀 / 去前缀
来源：http://hz.gogol.net.cn/gtgwbbgjiv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jinqigufen.top/gttmeblncb.html

[R26] 命令替换
来源：http://hz.zhaomingkeji.xyz/gtishlqonm.html

now=$(date +%F); echo "$now"
来源：http://hz.dianchejie.cn/gtxlahmwnj.html

[R27] 算术展开
来源：http://hz.ydjk.org.cn/gtkparzxmz.html

echo $((1 + 2 * 3))
来源：http://hz.jiagoushi.top/gtfgxlrusn.html

[R28] 浮点运算
来源：http://hz.feifeiyinyue.top/gtjljbvler.html

echo "scale=2; 10/3" | bc
来源：http://hz.dianchejie.cn/gtrykbpykx.html

[R29] 定义函数
来源：http://hz.hfpthk.cn/gthkcbuujd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shuidangran.top/gtixonaqvy.html

[R30] 函数返回状态码
来源：http://hz.yueranfly.top/gtzhqaysjc.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sufxvd.cn/gtdbikjxws.html

[R31] 局部变量
来源：http://hz.jianghu66.top/gttwnakcla.html

f() { local x=1; echo "$x"; }
来源：http://hz.chenzaomai.com/gtqxryykqg.html

[R32] 参数个数校验
来源：http://hz.xinyue.icu/gtuiyiapsx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cqqwz.cn/gtmvhobwlm.html

[R33] 捕获错误并提示行号
来源：http://hz.feifeiyinyue.top/gtzihvugcb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.guannengcc.top/gtqfdzflfy.html

[R34] 退出时清理
来源：http://hz.xuetiantiany.cn/gtuhkrkrws.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yangfankeji.com/gtcyhpqofp.html

[R35] 后台执行并等待
来源：http://hz.dianchejie.cn/gtmapqpdsk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cucudq.cn/gtmhfztrtb.html

[R36] 并发执行多个任务
来源：http://hz.yonumen.top/gtllviwvsw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xuetiantiany.cn/gtzmfvnigx.html

[R37] 把输出赋给变量
来源：http://hz.xingfuxueyuan.xyz/gtybzedcaa.html

files=$(ls -1)
来源：http://hz.zdqjudy.top/gtghertbps.html

[R38] 管道串联
来源：http://hz.52xcode.cn/gtqkgeueiv.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jyoumei.cn/gtdrcexvtz.html

[R39] 重定向标准输出与错误
来源：http://hz.ybcxt.top/gtnpwtztpm.html

cmd > out.log 2>&1
来源：http://hz.yueranfly.top/gtkrsluyvs.html

[R40] 追加写日志
来源：http://hz.daria6918.cn/gtvzrzlqxy.html

echo "log" >> out.log
来源：http://hz.gotoacloud.top/gtvkoamstf.html

[R41] 丢弃输出
来源：http://hz.xuanzx.com/gtzrywtume.html

cmd >/dev/null 2>&1
来源：http://hz.9152youxi.cn/gtxnmpeusm.html

[R42] 输入重定向
来源：http://hz.yj202588.top/gtniutbddr.html

wc -l < a.txt
来源：http://hz.wangshuangyany.cn/gtdlsfqyhx.html

[R43] 按名字查找文件
来源：http://hz.yuxming.cn/gtgsuojfcd.html

find . -name "*.log" -type f
来源：http://hz.chenzaomai.com/gtqpleyemk.html

[R44] 按修改时间查找
来源：http://hz.sweek.top/gtqynfkkiv.html

find . -mtime -7 -type f
来源：http://hz.iojbl.cn/gthkxrdsml.html

[R45] 批量删除
来源：http://hz.yvedp.cn/gtyscfkslk.html

find . -name "*.tmp" -delete
来源：http://hz.sweek.top/gtjmvhtdij.html

[R46] 递归替换文件内容
来源：http://hz.snrcjt.cn/gtkokclqfq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jinghuilouyu.cn/gttasvylms.html

[R47] sed 单行替换
来源：http://hz.xuanzx.com/gthveaxplb.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.birdmap.top/gtewtjfxvl.html

[R48] awk 取指定列
来源：http://hz.chenzaomai.com/gtiigpscmz.html

awk '{print $1, $3}' a.txt
来源：http://hz.hongshengwenyu.top/gtxmergref.html

[R49] awk 带条件
来源：http://hz.gogol.net.cn/gtldtrlrdf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhiwuduotai.top/gtplbaszgo.html

[R50] awk 求和
来源：http://hz.sufxvd.cn/gtpliwpxjt.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.0kj1m.cn/gtybohakgs.html

[R51] 排序去重取前几
来源：http://hz.gzhubu.top/gtboanzduy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jlsjyb.cn/gtecrnuxps.html

[R52] 统计行数
来源：http://hz.xingfuxueyuan.xyz/gtwxreynrf.html

wc -l a.txt
来源：http://hz.hfpthk.cn/gtawamezwx.html

[R53] 查看文件头与实时尾
来源：http://hz.xziqi.cn/gtdyaudqqw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.9152youxi.cn/gtfucbejyc.html

[R54] 比较两个文件
来源：http://hz.tanke756.top/gtxkezjdml.html

diff a.txt b.txt
来源：http://hz.xziqi.cn/gtjcfuybeo.html

[R55] 压缩与解压
来源：http://hz.jqgfzy.top/gtcxnjagoc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.aizwys.cn/gtkjcdhjbr.html

[R56] 远程拷贝
来源：http://hz.hongshengwenyu.top/gtdxtwmpgg.html

scp file user@host:/path/
来源：http://hz.pengpengdd.cyou/gtrbothseb.html

[R57] 远程执行命令
来源：http://hz.yuxming.cn/gtbtiusgtv.html

ssh user@host 'uptime'
来源：http://hz.316326.xyz/gtyrxlfkan.html

[R58] 下载文件
来源：http://hz.pycfn.com/gtjcehjsio.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shzxlz.cn/gtrzzbnycv.html

[R59] 发 POST JSON
来源：http://hz.aibaodan.cn/gtzyzijccs.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.guannengcc.top/gtzfqixcmu.html

[R60] 只看 HTTP 状态码
来源：http://hz.jlsjyb.cn/gtnckjtxjf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.tianlin.xyz/gtdbomegzl.html

[R61] 磁盘占用
来源：http://hz.yueranfly.top/gtvtqnchzj.html

df -h;  du -sh *
来源：http://hz.xuetiantiany.cn/gtulljlyxo.html

[R62] 找最占空间的文件
来源：http://hz.yonumen.top/gthzoocwru.html

du -ah . | sort -rh | head -10
来源：http://hz.zdqjudy.top/gtxwrmbpwj.html

[R63] 内存与进程
来源：http://hz.yueranfly.top/gtiztpqfxo.html

free -h;  ps aux | grep nginx
来源：http://hz.ydjk.org.cn/gtxnbckdcr.html

[R64] 结束进程
来源：http://hz.xuetiantiany.cn/gtzfkzqzoe.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hysaishi.cn/gtchhukxlf.html

[R65] 查看端口占用
来源：http://hz.jinqigufen.top/gtxekolnfn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.gzhubu.top/gtcxfguolq.html

[R66] 定时任务
来源：http://hz.zycfv.cn/gtvxrsztaw.html

crontab -e;  crontab -l
来源：http://hz.316326.xyz/gtngeqzpqj.html

[R67] 生成随机十六进制串
来源：http://hz.0kj1m.cn/gtkksfonyd.html

openssl rand -hex 16
来源：http://hz.gzhubu.top/gtnleupnqc.html

[R68] 计算文件校验值
来源：http://hz.zhengqikj.top/gtwrkizrvf.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.wangdashe.top/gtrnyuwppa.html

[R69] 生成随机密码
来源：http://hz.mhx1999.top/gtnvtwhrus.html

head -c 16 /dev/urandom | base64
来源：http://hz.c1oappe.top/gthkseqqyn.html

[R70] 时间戳与互转
来源：http://hz.shuidangran.top/gtugeoetgx.html

date +%s;  date -d @1700000000
来源：http://hz.yuanzhike.top/gtrrskkhmf.html

[R71] 日期格式化
来源：http://hz.xuanzx.com/gtlpuiibuv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.chenjidiqi.icu/gtzfaphsex.html

[R72] 等待端口就绪
来源：http://hz.andypj.xyz/gtvjukidla.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.daxiang520.top/gtcjlliycb.html

[R73] 分割大日志
来源：http://hz.ywan-chungtsiang.top/gtxnyjpkjl.html

split -l 1000 big.log part_
来源：http://hz.xingfuxueyuan.xyz/gtweypexwg.html

[R74] 批量重命名
来源：http://hz.jyoumei.cn/gtivjbbpsr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.daria6918.cn/gttpjslect.html

[R75] 导出环境变量
来源：http://hz.ydzc1.top/gtvlpfkome.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.mhx1999.top/gtqpfeqzej.html

[R76] 使用临时文件
来源：http://hz.shuidangran.top/gtjmkfihye.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zycfv.cn/gtriawuzib.html

[R77] 读取用户输入
来源：http://hz.zhoulong.xyz/gtlbdpgiis.html

read -rp "请输入: " ans
来源：http://hz.gotoacloud.top/gtodwkovvt.html

[R78] 交互式菜单
来源：http://hz.ppjwa.cn/gtjcfygyap.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ybcxt.top/gtwlyyootc.html

[R79] 解析命令行选项
来源：http://hz.shuidangran.top/gttvyoxlkl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xylfe.cn/gtzwdgrbni.html

[R80] 查看脚本执行耗时
来源：http://hz.hfpthk.cn/gtguytgbqr.html

time ./run.sh
来源：http://hz.tanke756.top/gtbjmcrllj.html

================================================================================
来源：http://hz.hfpthk.cn/gtctamcrla.html

S. C / C++ 专题
来源：http://hz.jiagoushi.top/gtrozqaihv.html

================================================================================
来源：http://hz.ehwqpu.com/gtmpvkiyin.html

[S01] C：Hello World
来源：http://hz.cashguo.top/gtgmgwatrb.html

#include <stdio.h>
来源：http://hz.hywenlv.cn/gtnocqbmrs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.chenlongwang.top/gtskigpahh.html

[S02] C：变量与格式化输出
来源：http://hz.ydzc1.top/gtffmzsdlf.html

int a = 10; printf("%d\n", a);
来源：http://hz.jinqigfzy.top/gtdacbkdii.html

[S03] C：读入整数
来源：http://hz.ywan-chungtsiang.top/gtoeqrqesv.html

int x; scanf("%d", &x);
来源：http://hz.xylfe.cn/gthsgaddgo.html

[S04] C：字符串复制
来源：http://hz.chenzaomai.com/gtfyksmuej.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jianghu66.top/gtrhucpnjx.html

[S05] C：字符串长度
来源：http://hz.jiagoushi.top/gtdrntztlq.html

strlen(s)
来源：http://hz.hongshengwenyu.top/gtdjdxnuly.html

[S06] C：字符串比较
来源：http://hz.yongpay.top/gtxdihmkau.html

strcmp(a, b) == 0
来源：http://hz.quarkkingdee.top/gtuoycnrwf.html

[S07] C：数组遍历求和
来源：http://hz.quarkkingdee.top/gtovveoloo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhaomingkeji.xyz/gtrhavrnhq.html

[S08] C：动态内存分配与释放
来源：http://hz.hywenlv.cn/gtdlzbrjsb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhijiandao.cn/gtjlyvsqbk.html

[S09] C：结构体定义与初始化
来源：http://hz.316326.xyz/gtbqskanws.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.dianchejie.cn/gteqzvhaps.html

[S10] C：指针与解引用
来源：http://hz.xuetiantiany.cn/gtxdqctfsr.html

int *p = &a;  *p = 5;
来源：http://hz.ehwqpu.com/gtjjyxncjs.html

[S11] C：逐行读文件
来源：http://hz.ydzc1.top/gtavorrwwj.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jyoumei.cn/gtvkftjcxr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.tanke756.top/gtzrlukbjx.html

fclose(f);
来源：http://hz.yueranfly.top/gtxrjsbail.html

[S12] C：写文件
来源：http://hz.cdnleiting.top/gtiwfcpmkv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.0kj1m.cn/gtcfxiloto.html

[S13] C：宏定义
来源：http://hz.jiagoushi.top/gtzvqsbwcw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yvedp.cn/gtdcluzcfc.html

[S14] C：枚举
来源：http://hz.zhongyouzk.top/gtuodooqvi.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.mhx1999.top/gtzdlernxt.html

[S15] C：类型转换
来源：http://hz.aizwys.cn/gtmsdohqbt.html

(double) a / b
来源：http://hz.smart0.xyz/gtjwzsyuei.html

[S16] C：位操作置位
来源：http://hz.hywenlv.cn/gtsoopkoqo.html

x |= (1 << 3);
来源：http://hz.nanxuanxn.top/gtvciegbdg.html

[S17] C：安全拼接字符串
来源：http://hz.guannengcc.top/gtxlhpknnr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ydjk.org.cn/gtowboxmma.html

[S18] C：命令行参数
来源：http://hz.aibaodan.cn/gthgtfuvog.html

int main(int argc, char **argv)
来源：http://hz.chenlongwang.top/gtmncfxyla.html

[S19] C：快速排序
来源：http://hz.yj202588.top/gtjsebwwyd.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhoulong.xyz/gtqseyqgdw.html

[S20] C：二分查找
来源：http://hz.0kj1m.cn/gtczhtysmx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yj20258.top/gtvbociktx.html

[S21] C：字符类别判断
来源：http://hz.zhengqikj.top/gtpbolivus.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.andypj.xyz/gtipnfqtst.html

[S22] C：字符串转数字
来源：http://hz.yj202588.top/gtohrtdvdu.html


<!-- 参考信息 -->