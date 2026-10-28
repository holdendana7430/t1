代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jianghu66.top/gthmekctqp.html

[Q50] 批量更新
来源：http://hz.jiagoushi.top/gttkngojwh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jinqigfzy.top/gthphacprk.html

[Q51] 用子查询更新
来源：http://hz.zhongyouzk.top/gtfugeluqw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hammf.cn/gtsuhrvjqv.html

[Q52] 删除指定行
来源：http://hz.ywan-chungtsiang.top/gtslqdyetz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hnqzz.top/gtltvvpmav.html

[Q53] 按条件删除
来源：http://hz.aibaodan.cn/gttaojgbma.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.sxryk.cn/gtutsitisq.html

[Q54] 清空表
来源：http://hz.jianghu66.top/gtafgbbpxb.html

TRUNCATE TABLE logs;
来源：http://hz.shangyingyoupin.top/gtneehxikd.html

[Q55] 排名（并列占位）
来源：http://hz.xylfe.cn/gtssqvlpuz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhiwuduotai.top/gtfqjmxovd.html

[Q56] 密集排名（并列不占位）
来源：http://hz.nanxinkj.top/gtefdpjmwi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.daxiang520.top/gtmqbvfnjl.html

[Q57] 行号
来源：http://hz.kuanghao11.cn/gtqpfoddyo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cheryme.top/gtpqqsqpqu.html

[Q58] 累计求和
来源：http://hz.zhijiandao.cn/gtyhbdeqvq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.nanxinkj.top/gtgbowezyg.html

[Q59] 分组内累计
来源：http://hz.xuanzx.com/gtljeyoild.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yj202588.top/gtequsymsj.html

[Q60] 取上一行 / 下一行
来源：http://hz.wangdashe.top/gtovbkkqpa.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.snrcjt.cn/gtgvicmmck.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.guowangkeji.top/gtuagfwcfv.html

[Q61] 移动平均
来源：http://hz.redwolf501.top/gtshdiiyce.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.chenzaomai.com/gtimnnezae.html

[Q62] 分组占比
来源：http://hz.yj202588.top/gthxkpyhac.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.52xcode.cn/gtbvlcdqvk.html

[Q63] 开启事务
来源：http://hz.yj202588.top/gtsylvcgxq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cqqwz.cn/gtbglhhecq.html

[Q64] 提交事务
来源：http://hz.bjfxy.top/gtfeworqff.html

COMMIT;
来源：http://hz.guannengcc.top/gtcatpawiz.html

[Q65] 回滚事务
来源：http://hz.yj20258.top/gtfdrrpjmq.html

ROLLBACK;
来源：http://hz.jqgufenzy.top/gtvomiwugs.html

[Q66] 行锁查询
来源：http://hz.bjfxy.top/gtuvdiobgh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yuxming.cn/gtkafsgcak.html

[Q67] 设置隔离级别
来源：http://hz.daria6918.cn/gtfzrkjkev.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ybcxt.top/gtsihsagpp.html

[Q68] 保存点
来源：http://hz.kuanghao11.cn/gtyowlabwn.html

SAVEPOINT sp1;
来源：http://hz.9152youxi.cn/gtzvxrldya.html

ROLLBACK TO sp1;
来源：http://hz.guannengcc.top/gtgirplrwc.html

[Q69] 查看执行计划
来源：http://hz.smart0.xyz/gtcoxptorg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.wangdashe.top/gtgwlovolk.html

[Q70] 更新统计信息
来源：http://hz.nanxuanxn.top/gtbsfruuhg.html

ANALYZE TABLE users;
来源：http://hz.yongpay.top/gttqwpizdi.html

[Q71] 查看建表语句
来源：http://hz.9152youxi.cn/gtowsqacyv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hysaishi.cn/gtqfctuqxd.html

[Q72] 查看索引
来源：http://hz.zhoulong.xyz/gtfefijkvu.html

SHOW INDEX FROM users;
来源：http://hz.shuidangran.top/gtbagbxumy.html

[Q73] 查看表状态
来源：http://hz.xziqi.cn/gtsqylkolh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jqgufenzy.top/gtejguqglf.html

[Q74] 强制使用索引
来源：http://hz.jinyuanbaomall.cn/gtolvyfhrw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ybcxt.top/gtaeqgucun.html

[Q75] 日期格式化
来源：http://hz.ehwqpu.com/gtqsroiget.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xuetiantiany.cn/gthfplxbzt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hongshengwenyu.top/gtaglttlmm.html

[Q76] 按天统计
来源：http://hz.zhengqikj.top/gtxzwzxias.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.nwbrower.top/gtvnvextvl.html

[Q77] 时间加减
来源：http://hz.chenzaomai.com/gtscrqnuuk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.xuetiantiany.cn/gtltbhapia.html

[Q78] 当前时间
来源：http://hz.hongshengwenyu.top/gtrqfwyilv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jqgfzy.top/gtungbodog.html

[Q79] 字符串拼接
来源：http://hz.feifeiyinyue.top/gtxiyoraqd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.tianlin.xyz/gtonmiyjna.html

[Q80] 字符串截取
来源：http://hz.hywenlv.cn/gtyxxeqhvn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cucudq.cn/gtscxmcpgj.html

[Q81] 字符串替换
来源：http://hz.bjfxy.top/gthbaiqkrt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhixingplan.top/gtkpfgaafx.html

[Q82] 字符长度与字节长度
来源：http://hz.tanke756.top/gtqrkpqnrv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.nanxuanxn.top/gtccvzlgoi.html

[Q83] 大小写转换
来源：http://hz.pycfn.com/gthqbwsjwl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.c1oappe.top/gtvompqukc.html

[Q84] 去除首尾空格
来源：http://hz.meibo888.top/gteojpxfqa.html

SELECT TRIM(name) FROM users;
来源：http://hz.sysykeji.top/gtwdgrofsi.html

[Q85] 数值取整
来源：http://hz.meibo888.top/gtfszrhygj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hnqzz.top/gthkuuqdbd.html

[Q86] 读取 JSON 字段
来源：http://hz.52xcode.cn/gtxgneartf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yj202588.top/gtelmjptkz.html

[Q87] JSON 字段做条件
来源：http://hz.sxryk.cn/gtuycwopum.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.shanyushiyangkeji.top/gtylnwfsxm.html

[Q88] 行转列（条件聚合）
来源：http://hz.gzhubu.top/gtbmsdramq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hysaishi.cn/gternmqhmi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ivvv.top/gtrufatsmh.html

[Q89] 判断表是否存在
来源：http://hz.daria6918.cn/gtbeffyffe.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.chenjidiqi.icu/gtjyjladzg.html

[Q90] 生成序号列
来源：http://hz.nanxuanxn.top/gtxovgffpk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.bjfxy.top/gtgnrxzfku.html

================================================================================
来源：http://hz.redwolf501.top/gtoielkyno.html

R. Bash 专题
来源：http://hz.redwolf501.top/gtmuevutbc.html

================================================================================
来源：http://hz.daxiang520.top/gtorsqrfsw.html

[R01] shebang 与严格模式
来源：http://hz.xziqi.cn/gtdgtsyqhj.html

#!/usr/bin/env bash
来源：http://hz.c1oappe.top/gtxdlrfrln.html

set -euo pipefail
来源：http://hz.aibaodan.cn/gtfmtybweh.html

[R02] 变量赋值与使用
来源：http://hz.hnxiangtu.top/gtlufjxeng.html

name="Tom"; echo "$name"
来源：http://hz.jianghu66.top/gtgqwdkkfh.html

[R03] 只读变量
来源：http://hz.ppjwa.cn/gtzfutbdja.html

readonly PI=3.14
来源：http://hz.vqdsnc.cn/gtylmvojus.html

[R04] 位置参数
来源：http://hz.hnxiangtu.top/gtebodkxhs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.haohaochexian.top/gtnctehotb.html

[R05] 参数默认值
来源：http://hz.zhongyouzk.top/gtvjyyidts.html

name="${1:-default}"
来源：http://hz.ppjwa.cn/gtkivwxbst.html

[R06] 判断命令是否存在
来源：http://hz.guowangkeji.top/gtrxmhhydu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yj20258.top/gtnrlsqsij.html

[R07] if 判断文件
来源：http://hz.shanyushiyangkeji.top/gtnrkuncxo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.chenlongwang.top/gtfjupfiwx.html

[R08] 数值比较
来源：http://hz.yueranfly.top/gtugfcnwrw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ppjwa.cn/gtqdyltevg.html

[R09] 字符串比较
来源：http://hz.hammf.cn/gtihcgzcyu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yuanzhike.top/gtwobcrcmg.html

[R10] 正则匹配
来源：http://hz.chenlongwang.top/gttfmornyk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cdnleiting.top/gtrlbvjzut.html

[R11] case 多分支
来源：http://hz.yj20258888.top/gtrxwnnith.html

case "$1" in
来源：http://hz.jqgfzy.top/gtletkrciv.html

start) echo "启动" ;;
来源：http://hz.nwbrower.top/gtfztzazec.html

stop)  echo "停止" ;;
来源：http://hz.ydzc1.top/gtdbsongfu.html

*)     echo "未知命令" ;;
来源：http://hz.gotoacloud.top/gterbucqgl.html

esac
来源：http://hz.zhengqikj.top/gtdnygtfit.html

[R12] for 遍历文件
来源：http://hz.zhijiandao.cn/gtaxicmpwr.html

for f in *.txt; do echo "$f"; done
来源：http://hz.chenlongwang.top/gtolgpqclo.html

[R13] for 计数循环
来源：http://hz.jinqigufen.top/gtcmhaepfa.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.meibo888.top/gtpxomikfi.html

[R14] C 风格 for
来源：http://hz.jinyuanbaomall.cn/gtfhrvkvrk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shuidangran.top/gtvlhydald.html

[R15] while 逐行读文件
来源：http://hz.snrcjt.cn/gtbutzthia.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.gaohongyu789.top/gtjunixiaf.html

[R16] until 等待条件
来源：http://hz.svipenyu.cn/gtfhgpxujw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.wangdashe.top/gtkvdntmsd.html

[R17] 数组定义与取值
来源：http://hz.xuanzx.com/gttcfrtcsc.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hongshengwenyu.top/gtnmhkkjtg.html

[R18] 遍历数组
来源：http://hz.ybcxt.top/gtsqjnknss.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.gotoacloud.top/gtsfktcixn.html

[R19] 数组长度
来源：http://hz.iojbl.cn/gtwdwpnpwu.html

echo "${#arr[@]}"
来源：http://hz.xziqi.cn/gtwognqdqx.html

[R20] 关联数组（字典）
来源：http://hz.tianlin.xyz/gtbkgjlptm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.sweek.top/gtbdzvjdfu.html

[R21] 字符串长度
来源：http://hz.birdmap.top/gtgokuurba.html

echo "${#s}"
来源：http://hz.yj20258.top/gtaxryotyu.html

[R22] 截取子串
来源：http://hz.jqgfzy.top/gthirxdtsx.html

echo "${s:0:5}"
来源：http://hz.52xcode.cn/gtgfilrpio.html

[R23] 字符串替换
来源：http://hz.gzhubu.top/gteogavrxm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jqgfzy.top/gtcsesvczj.html

[R24] 大小写转换
来源：http://hz.chenlongwang.top/gtgjltezhp.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.andypj.xyz/gtljknfevk.html

[R25] 去后缀 / 去前缀
来源：http://hz.9152youxi.cn/gtbsvazzzj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.wangdashe.top/gtedtpkbnx.html

[R26] 命令替换
来源：http://hz.yj202588.top/gtsanpggto.html

now=$(date +%F); echo "$now"
来源：http://hz.xingfuxueyuan.xyz/gttftfmnrr.html

[R27] 算术展开
来源：http://hz.mhx1999.top/gtiasllyfh.html

echo $((1 + 2 * 3))
来源：http://hz.gzhubu.top/gtkwtthdfc.html

[R28] 浮点运算
来源：http://hz.aibaodan.cn/gtrenhlytf.html

echo "scale=2; 10/3" | bc
来源：http://hz.feifeiyinyue.top/gtykvejuwd.html

[R29] 定义函数
来源：http://hz.yanxiufei.cn/gtfeqppclb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.guannengcc.top/gtesiyfewz.html

[R30] 函数返回状态码
来源：http://hz.hnxiangtu.top/gtjyooqmtv.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.birdmap.top/gtfuhzgqlo.html

[R31] 局部变量
来源：http://hz.ydjk.org.cn/gtmrhzehrj.html

f() { local x=1; echo "$x"; }
来源：http://hz.yangfankeji.com/gthhqjttpq.html

[R32] 参数个数校验
来源：http://hz.jinghuilouyu.cn/gtszhozsvf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.vqdsnc.cn/gtlqethpho.html

[R33] 捕获错误并提示行号
来源：http://hz.pengpengdd.cyou/gtvggjdqgm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.0kj1m.cn/gtqzplvcvt.html

[R34] 退出时清理
来源：http://hz.ivvv.top/gtoxbkjrxz.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.guowangkeji.top/gtjnagckpf.html

[R35] 后台执行并等待
来源：http://hz.nanxuanxn.top/gtxohexjbg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zycfv.cn/gttfrciyau.html

[R36] 并发执行多个任务
来源：http://hz.yj202588.top/gtntnquopn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.mhx1999.top/gtkxdgeqhn.html

[R37] 把输出赋给变量
来源：http://hz.haohaochexian.top/gtdckfihve.html

files=$(ls -1)
来源：http://hz.fengsongda.top/gtmxjqbbeu.html

[R38] 管道串联
来源：http://hz.hfpthk.cn/gteuyljzfh.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sxryk.cn/gtcjdwnybq.html

[R39] 重定向标准输出与错误
来源：http://hz.9152youxi.cn/gtlgldzalg.html

cmd > out.log 2>&1
来源：http://hz.ivvv.top/gtrpggmteq.html

[R40] 追加写日志
来源：http://hz.jinqigfzy.top/gtzoteodtl.html

echo "log" >> out.log
来源：http://hz.jinqigufen.top/gtrtltktxk.html

[R41] 丢弃输出
来源：http://hz.shzxlz.cn/gttnqfyobj.html

cmd >/dev/null 2>&1
来源：http://hz.hysaishi.cn/gtwteydyzr.html

[R42] 输入重定向
来源：http://hz.zhengqikj.top/gtrmndmxth.html

wc -l < a.txt
来源：http://hz.yanxiufei.cn/gtnjguaqeh.html

[R43] 按名字查找文件
来源：http://hz.yanxiufei.cn/gtcvzswlnj.html

find . -name "*.log" -type f
来源：http://hz.gzhubu.top/gtfyckxihv.html

[R44] 按修改时间查找
来源：http://hz.jqgufenzy.top/gtkdpnwjdn.html

find . -mtime -7 -type f
来源：http://hz.jinqigfzy.top/gtgjbipxtv.html

[R45] 批量删除
来源：http://hz.zhengqikj.top/gtdfmvtrzb.html

find . -name "*.tmp" -delete
来源：http://hz.andypj.xyz/gtsvjbpsdb.html

[R46] 递归替换文件内容
来源：http://hz.yvedp.cn/gthnfzwfpd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yuxming.cn/gtyoqyahva.html

[R47] sed 单行替换
来源：http://hz.chenlongwang.top/gtholbnycn.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ppjwa.cn/gtsthfegfo.html

[R48] awk 取指定列
来源：http://hz.fzhhl.top/gtriooqhjf.html

awk '{print $1, $3}' a.txt
来源：http://hz.vqdsnc.cn/gthyppjtxj.html

[R49] awk 带条件
来源：http://hz.ydjk.org.cn/gtdiidmtnw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhijiandao.cn/gtdivjzfvg.html

[R50] awk 求和
来源：http://hz.chenjidiqi.icu/gtopzzpgqd.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shzxlz.cn/gtrghbgqhc.html

[R51] 排序去重取前几
来源：http://hz.yongpay.top/gtjegdxaic.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.chenjidiqi.icu/gtfoziqsys.html

[R52] 统计行数
来源：http://hz.smart0.xyz/gtczbuzqlp.html

wc -l a.txt
来源：http://hz.shzxlz.cn/gtfxqbtgoq.html

[R53] 查看文件头与实时尾
来源：http://hz.bjfxy.top/gtevayptkj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.dashuyun.cn/gtkozjqgah.html

[R54] 比较两个文件
来源：http://hz.yonumen.top/gtrpavqcsn.html

diff a.txt b.txt
来源：http://hz.gzhubu.top/gtgzxzsbbq.html

[R55] 压缩与解压
来源：http://hz.wangdashe.top/gtzzmfnpuf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhengqikj.top/gttitqkxzn.html

[R56] 远程拷贝
来源：http://hz.yuanzhike.top/gtkpbpkcxx.html

scp file user@host:/path/
来源：http://hz.shanyushiyangtech.top/gthujcbppw.html

[R57] 远程执行命令
来源：http://hz.havefunace.top/gtsnprriya.html

ssh user@host 'uptime'
来源：http://hz.jinyuanbaomall.cn/gtngntstqw.html

[R58] 下载文件
来源：http://hz.redwolf501.top/gtuglmtdom.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.haohaochexian.top/gtwbmvlocz.html

[R59] 发 POST JSON
来源：http://hz.aizwys.cn/gtcnjcmlzp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shangyingyoupin.top/gtxybluvmi.html

[R60] 只看 HTTP 状态码
来源：http://hz.havefunace.top/gtfuvomcxb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.svipenyu.cn/gtgnarorkq.html

[R61] 磁盘占用
来源：http://hz.haohaochexian.top/gtxpggxopo.html

df -h;  du -sh *
来源：http://hz.yueranfly.top/gthhdondme.html

[R62] 找最占空间的文件
来源：http://hz.aibaodan.cn/gtfnvmtjlk.html

du -ah . | sort -rh | head -10
来源：http://hz.yonumen.top/gtjycnwplu.html

[R63] 内存与进程
来源：http://hz.gaohongyu789.top/gtupqseccg.html

free -h;  ps aux | grep nginx
来源：http://hz.jlsjyb.cn/gtpgheasss.html

[R64] 结束进程
来源：http://hz.daxiang520.top/gtbbjqeswn.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xuanzx.com/gtekjlenyz.html

[R65] 查看端口占用
来源：http://hz.jyoumei.cn/gtqkfxtgzh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.tanke756.top/gtvndwlted.html

[R66] 定时任务
来源：http://hz.jiagoushi.top/gtzyczgfaw.html

crontab -e;  crontab -l
来源：http://hz.ivvv.top/gtnzobdniw.html

[R67] 生成随机十六进制串
来源：http://hz.iojbl.cn/gtyaqhcnqv.html

openssl rand -hex 16
来源：http://hz.tanke756.top/gtlxqyqurp.html

[R68] 计算文件校验值
来源：http://hz.nanxinkj.top/gtbtrggihm.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hammf.cn/gtxgqpttng.html

[R69] 生成随机密码
来源：http://hz.tanke756.top/gtwrfbwzac.html

head -c 16 /dev/urandom | base64
来源：http://hz.tanke756.top/gtduefbjbr.html

[R70] 时间戳与互转
来源：http://hz.shuidangran.top/gtydwdjpsq.html

date +%s;  date -d @1700000000
来源：http://hz.xziqi.cn/gtyheeuvbm.html

[R71] 日期格式化
来源：http://hz.jiagoushi.top/gtflbdoxeh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yj20258.top/gtwnihubcm.html

[R72] 等待端口就绪
来源：http://hz.hnqzz.top/gtfwtpegik.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yj20258888.top/gteohgvthd.html

[R73] 分割大日志
来源：http://hz.wangshuangyany.cn/gtnaxzjorl.html

split -l 1000 big.log part_
来源：http://hz.chenzaomai.com/gtwkjaxetb.html

[R74] 批量重命名
来源：http://hz.chenlongwang.top/gtdjjzxxcr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jiagoushi.top/gtqiqweqxk.html

[R75] 导出环境变量
来源：http://hz.gzhubu.top/gtevolvear.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.gotoacloud.top/gthojzvsau.html

[R76] 使用临时文件
来源：http://hz.daxiang520.top/gtruxqmnkx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinqigufen.top/gtsyifvwll.html

[R77] 读取用户输入
来源：http://hz.ppjwa.cn/gtrrdvzeuw.html

read -rp "请输入: " ans
来源：http://hz.shuidangran.top/gtisarmezx.html

[R78] 交互式菜单
来源：http://hz.zdqjudy.top/gtuuwmaabz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xinyue.icu/gtnnzpypes.html

[R79] 解析命令行选项
来源：http://hz.dashuyun.cn/gtbvcfqvch.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xuetiantiany.cn/gttnddztwn.html

[R80] 查看脚本执行耗时
来源：http://hz.dashuyun.cn/gtyoirchir.html

time ./run.sh
来源：http://hz.tianlin.xyz/gtduscudtt.html

================================================================================
来源：http://hz.chenzaomai.com/gtsdynmjws.html

S. C / C++ 专题
来源：http://hz.jinyuanbaomall.cn/gtptnsakmr.html

================================================================================
来源：http://hz.cashguo.top/gtfzjogcfi.html

[S01] C：Hello World
来源：http://hz.jqgfzy.top/gtjikaexrh.html

#include <stdio.h>
来源：http://hz.sxryk.cn/gtfoeotyvk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.sufxvd.cn/gtvtwylltk.html

[S02] C：变量与格式化输出
来源：http://hz.haohaochexian.top/gtdgfhwvwa.html

int a = 10; printf("%d\n", a);
来源：http://hz.chenlongwang.top/gtnrihnxxq.html

[S03] C：读入整数
来源：http://hz.gogol.net.cn/gtxxerzowg.html

int x; scanf("%d", &x);
来源：http://hz.jqgufenzy.top/gthjsvwhau.html

[S04] C：字符串复制
来源：http://hz.bjfxy.top/gtvclwxapu.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jiagoushi.top/gtbegjuqre.html

[S05] C：字符串长度
来源：http://hz.wangdashe.top/gtzvsdwbqh.html

strlen(s)
来源：http://hz.0kj1m.cn/gtcebdcixi.html

[S06] C：字符串比较
来源：http://hz.9152youxi.cn/gtwdlwnyyd.html

strcmp(a, b) == 0
来源：http://hz.fzhhl.top/gtawwpbegr.html

[S07] C：数组遍历求和
来源：http://hz.xingfuxueyuan.xyz/gtptiokuel.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.shzxlz.cn/gtdinpukzc.html

[S08] C：动态内存分配与释放
来源：http://hz.ivvv.top/gtcoxvwdad.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zycfv.cn/gtnmandoui.html

[S09] C：结构体定义与初始化
来源：http://hz.xingfuxueyuan.xyz/gtdzykzbkt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.nwbrower.top/gtzessxour.html

[S10] C：指针与解引用
来源：http://hz.zhiwuduotai.top/gtzncypaix.html

int *p = &a;  *p = 5;
来源：http://hz.dashuyun.cn/gtliboqscm.html

[S11] C：逐行读文件
来源：http://hz.jiagoushi.top/gtdsyhcjhh.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.dianchejie.cn/gtyebwitbs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jyoumei.cn/gtwrqfteby.html

fclose(f);
来源：http://hz.sysykeji.top/gtipmcsaka.html

[S12] C：写文件
来源：http://hz.jyoumei.cn/gtogahbaak.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yuxming.cn/gthcfaymkc.html

[S13] C：宏定义
来源：http://hz.yangfankeji.com/gtvqatvqlo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hongshengwenyu.top/gtpepkkmjt.html

[S14] C：枚举
来源：http://hz.ydzc1.top/gtwkgjckyo.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.guowangkeji.top/gtxbqcojfr.html

[S15] C：类型转换
来源：http://hz.tian-w.cn/gtpwzyrova.html

(double) a / b
来源：http://hz.0kj1m.cn/gtyheklndi.html

[S16] C：位操作置位
来源：http://hz.ywan-chungtsiang.top/gtushwcyhy.html

x |= (1 << 3);
来源：http://hz.havefunace.top/gtaolzwcig.html

[S17] C：安全拼接字符串
来源：http://hz.yonumen.top/gtbtygwcum.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yonumen.top/gtjyotxuwg.html

[S18] C：命令行参数
来源：http://hz.feifeiyinyue.top/gtvpkultgs.html

int main(int argc, char **argv)
来源：http://hz.fengsongda.top/gthztrndjf.html

[S19] C：快速排序
来源：http://hz.pycfn.com/gtwjvuueuj.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.chenlongwang.top/gtwshergnz.html

[S20] C：二分查找
来源：http://hz.xziqi.cn/gtbljwhcvv.html


<!-- 参考信息 -->