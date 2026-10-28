代发 wailian999

[Q48] CTE 公用表表达式
来源：http://hz.birdmap.top/gtgsaprdof.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yueranfly.top/gtwkvdmefm.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.mhx1999.top/gtbnrbazlp.html

[Q49] 更新单行
来源：http://hz.pengpengdd.cyou/gtmjfqoecc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.gogol.net.cn/gtiidilbtz.html

[Q50] 批量更新
来源：http://hz.zycfv.cn/gtktkdhbyb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yj202588.top/gtktyrtdpi.html

[Q51] 用子查询更新
来源：http://hz.sysykeji.top/gtpirpdmhs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ybcxt.top/gtihsprktn.html

[Q52] 删除指定行
来源：http://hz.andypj.xyz/gtevbbdrfr.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yj20258888.top/gtyqtdervr.html

[Q53] 按条件删除
来源：http://hz.tianlin.xyz/gthzjolgaz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jianghu66.top/gtsunzcqcj.html

[Q54] 清空表
来源：http://hz.jinqigufen.top/gtcgbtuliq.html

TRUNCATE TABLE logs;
来源：http://hz.sufxvd.cn/gtltfwulqz.html

[Q55] 排名（并列占位）
来源：http://hz.zhixingplan.top/gtsfznypxl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yonumen.top/gtcfmbfbbf.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xingfuxueyuan.xyz/gtevauuzlx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jiagoushi.top/gthtzpuocw.html

[Q57] 行号
来源：http://hz.dianchejie.cn/gtwhidhlwp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.c1oappe.top/gtcnluswsd.html

[Q58] 累计求和
来源：http://hz.redwolf501.top/gtcydaqigk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.gaohongyu789.top/gtlsdvodae.html

[Q59] 分组内累计
来源：http://hz.wangshuangyany.cn/gttokzepoh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hysaishi.cn/gtqatdotux.html

[Q60] 取上一行 / 下一行
来源：http://hz.cdnleiting.top/gtbjhgfvsc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.vqdsnc.cn/gthsshwyud.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.guowangkeji.top/gtawawzsym.html

[Q61] 移动平均
来源：http://hz.gogol.net.cn/gtayxrysjy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhoulong.xyz/gtzknnfwpd.html

[Q62] 分组占比
来源：http://hz.pycfn.com/gtrfnovige.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cdnleiting.top/gtkmjsqwzx.html

[Q63] 开启事务
来源：http://hz.jqgfzy.top/gtrzpiiwhs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yanxiufei.cn/gtdlfhwqae.html

[Q64] 提交事务
来源：http://hz.zhixingplan.top/gtirdbgiod.html

COMMIT;
来源：http://hz.birdmap.top/gtnxubvhuy.html

[Q65] 回滚事务
来源：http://hz.guowangkeji.top/gtqywkrbyn.html

ROLLBACK;
来源：http://hz.wangdashe.top/gtjaynvawj.html

[Q66] 行锁查询
来源：http://hz.chenlongwang.top/gtrumlpugh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.wangshuangyany.cn/gtbuxxxzbv.html

[Q67] 设置隔离级别
来源：http://hz.jqgufenzy.top/gtudlsfsbe.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.fzhhl.top/gtbtulujoq.html

[Q68] 保存点
来源：http://hz.gaohongyu789.top/gtchvyfiib.html

SAVEPOINT sp1;
来源：http://hz.gotoacloud.top/gtiwqqhrht.html

ROLLBACK TO sp1;
来源：http://hz.wangshuangyany.cn/gttufqpmls.html

[Q69] 查看执行计划
来源：http://hz.gotoacloud.top/gtammmeixb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yuanzhike.top/gtyytgarqe.html

[Q70] 更新统计信息
来源：http://hz.quarkkingdee.top/gtzkvclkxf.html

ANALYZE TABLE users;
来源：http://hz.jinyuanbaomall.cn/gtxifbvtuo.html

[Q71] 查看建表语句
来源：http://hz.jlsjyb.cn/gtmfuvynkt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jyoumei.cn/gtsyxumnpd.html

[Q72] 查看索引
来源：http://hz.zhoulong.xyz/gtasloiize.html

SHOW INDEX FROM users;
来源：http://hz.aizwys.cn/gtfynxihpz.html

[Q73] 查看表状态
来源：http://hz.ehwqpu.com/gtusznhhyl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ybcxt.top/gtuknxpwoi.html

[Q74] 强制使用索引
来源：http://hz.yuanzhike.top/gtnaxbucjo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jlsjyb.cn/gtamhzracq.html

[Q75] 日期格式化
来源：http://hz.feifeiyinyue.top/gtzqwewggr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jqgfzy.top/gteqyyajfh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.bjfxy.top/gtcydiibzl.html

[Q76] 按天统计
来源：http://hz.andypj.xyz/gtdeobkvbb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ppjwa.cn/gttxgwtovp.html

[Q77] 时间加减
来源：http://hz.chenjidiqi.icu/gthibuetgs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.wangshuangyany.cn/gtxnniqist.html

[Q78] 当前时间
来源：http://hz.sysykeji.top/gtgaonnqju.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hnqzz.top/gtoisungwx.html

[Q79] 字符串拼接
来源：http://hz.quarkkingdee.top/gtefnkmoca.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yongpay.top/gtdrivitfk.html

[Q80] 字符串截取
来源：http://hz.feifeiyinyue.top/gterivyukq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.aibaodan.cn/gtaneyzaau.html

[Q81] 字符串替换
来源：http://hz.shzxlz.cn/gtfomujihf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.gaohongyu789.top/gtwbierfyi.html

[Q82] 字符长度与字节长度
来源：http://hz.yueranfly.top/gtjkulisxa.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cheryme.top/gtzjwlbuvc.html

[Q83] 大小写转换
来源：http://hz.shanyushiyangkeji.top/gterrawhmr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xylfe.cn/gtjpqhqcrn.html

[Q84] 去除首尾空格
来源：http://hz.xingfuxueyuan.xyz/gtpegxcyir.html

SELECT TRIM(name) FROM users;
来源：http://hz.hammf.cn/gtiunbxjgs.html

[Q85] 数值取整
来源：http://hz.aibaodan.cn/gtermtrlfm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.fzhhl.top/gtgvilzgrp.html

[Q86] 读取 JSON 字段
来源：http://hz.yvedp.cn/gtoojrjgxl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.cheryme.top/gtploepvot.html

[Q87] JSON 字段做条件
来源：http://hz.hfpthk.cn/gtvlbufzrq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cucudq.cn/gtlmevyoai.html

[Q88] 行转列（条件聚合）
来源：http://hz.yuxming.cn/gtszaqdzqp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yuanzhike.top/gtaqqwvhii.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yueranfly.top/gtlwjcohoo.html

[Q89] 判断表是否存在
来源：http://hz.shanyushiyangtech.top/gthzcpuzxb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jinghuilouyu.cn/gtgxhpwulv.html

[Q90] 生成序号列
来源：http://hz.gotoacloud.top/gtgutynwwp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.pengpengdd.cyou/gtwjjuvgcw.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtogbqteyu.html

R. Bash 专题
来源：http://hz.havefunace.top/gtrikyyyry.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtqecfzdfq.html

[R01] shebang 与严格模式
来源：http://hz.kuanghao11.cn/gtjnjvjrfo.html

#!/usr/bin/env bash
来源：http://hz.ywan-chungtsiang.top/gtwppixpsm.html

set -euo pipefail
来源：http://hz.guannengcc.top/gtmawncdwj.html

[R02] 变量赋值与使用
来源：http://hz.dianchejie.cn/gtjdzkqdsm.html

name="Tom"; echo "$name"
来源：http://hz.shangyingyoupin.top/gtjmfjqauf.html

[R03] 只读变量
来源：http://hz.52xcode.cn/gtzniozbco.html

readonly PI=3.14
来源：http://hz.ydzc1.top/gtmazpbrlf.html

[R04] 位置参数
来源：http://hz.hysaishi.cn/gthchjslzw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xziqi.cn/gtgtcblyxe.html

[R05] 参数默认值
来源：http://hz.ydzc1.top/gtjqqgvmdd.html

name="${1:-default}"
来源：http://hz.gogol.net.cn/gtfmwgtknk.html

[R06] 判断命令是否存在
来源：http://hz.yueranfly.top/gtsmtxrhdi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhoulong.xyz/gtbldvhhcx.html

[R07] if 判断文件
来源：http://hz.daria6918.cn/gtwzpebupp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yanxiufei.cn/gthofemagm.html

[R08] 数值比较
来源：http://hz.birdmap.top/gtwelhjbxx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.aibaodan.cn/gtdtnjuppc.html

[R09] 字符串比较
来源：http://hz.316326.xyz/gtfhbooxpk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.bjfxy.top/gtqsvugcuk.html

[R10] 正则匹配
来源：http://hz.shanyushiyangkeji.top/gtlgyqsfhh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jianghu66.top/gtzaaerkwz.html

[R11] case 多分支
来源：http://hz.zhoulong.xyz/gtghrlxibm.html

case "$1" in
来源：http://hz.sweek.top/gtgdthnovn.html

start) echo "启动" ;;
来源：http://hz.tanke756.top/gtuxhnwtck.html

stop)  echo "停止" ;;
来源：http://hz.daria6918.cn/gtzkmlnnpy.html

*)     echo "未知命令" ;;
来源：http://hz.yangfankeji.com/gtasdeqvts.html

esac
来源：http://hz.cashguo.top/gtdstchbrw.html

[R12] for 遍历文件
来源：http://hz.tianlin.xyz/gtsfquqjqu.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yanxiufei.cn/gtktitvmfh.html

[R13] for 计数循环
来源：http://hz.wangshuangyany.cn/gtecvsktiu.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ivvv.top/gtdnhfhjtm.html

[R14] C 风格 for
来源：http://hz.shangyingyoupin.top/gtszmbsohd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhongyouzk.top/gttxikjzne.html

[R15] while 逐行读文件
来源：http://hz.gogol.net.cn/gtefzzriso.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.cqqwz.cn/gtudkrsfha.html

[R16] until 等待条件
来源：http://hz.zhiwuduotai.top/gthrszadgw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.cqqwz.cn/gtdvcminzz.html

[R17] 数组定义与取值
来源：http://hz.gzhubu.top/gtlokfaajr.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cqqwz.cn/gtkwgznqwz.html

[R18] 遍历数组
来源：http://hz.jqgufenzy.top/gtlrzcqzpo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yangfankeji.com/gtstodiniw.html

[R19] 数组长度
来源：http://hz.c1oappe.top/gtwtpyyxia.html

echo "${#arr[@]}"
来源：http://hz.yongpay.top/gtxngyzmzc.html

[R20] 关联数组（字典）
来源：http://hz.svipenyu.cn/gtcqvzbrek.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cheryme.top/gtaqazkvhz.html

[R21] 字符串长度
来源：http://hz.yj20258888.top/gtuboqvits.html

echo "${#s}"
来源：http://hz.hammf.cn/gtxllhjpmg.html

[R22] 截取子串
来源：http://hz.pycfn.com/gtzekdhicp.html

echo "${s:0:5}"
来源：http://hz.chenzaomai.com/gtgyfrlipk.html

[R23] 字符串替换
来源：http://hz.zhongyouzk.top/gtqaywwvfj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhiwuduotai.top/gtofifkosk.html

[R24] 大小写转换
来源：http://hz.xziqi.cn/gtfqbvfkxo.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj202588.top/gtuiozynyd.html

[R25] 去后缀 / 去前缀
来源：http://hz.ivvv.top/gtkxgshjbb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shuidangran.top/gtfbskogkr.html

[R26] 命令替换
来源：http://hz.aizwys.cn/gtitsvwjft.html

now=$(date +%F); echo "$now"
来源：http://hz.shanyushiyangkeji.top/gttcootssn.html

[R27] 算术展开
来源：http://hz.cheryme.top/gtwprbgxbf.html

echo $((1 + 2 * 3))
来源：http://hz.shangyingyoupin.top/gtfasqhwjc.html

[R28] 浮点运算
来源：http://hz.meibo888.top/gtkmpzymcc.html

echo "scale=2; 10/3" | bc
来源：http://hz.yangfankeji.com/gtgwolzoda.html

[R29] 定义函数
来源：http://hz.yuanzhike.top/gtybmovsga.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.aibaodan.cn/gtrnvzgcop.html

[R30] 函数返回状态码
来源：http://hz.cucudq.cn/gtfhrycijf.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xuetiantiany.cn/gtpyykbyqj.html

[R31] 局部变量
来源：http://hz.dianchejie.cn/gtcnkiexni.html

f() { local x=1; echo "$x"; }
来源：http://hz.0kj1m.cn/gtytztikxf.html

[R32] 参数个数校验
来源：http://hz.aibaodan.cn/gttcwxvoms.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yvedp.cn/gtkybhiigp.html

[R33] 捕获错误并提示行号
来源：http://hz.xingfuxueyuan.xyz/gtuffkhbdv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.316326.xyz/gtptcuoram.html

[R34] 退出时清理
来源：http://hz.xuetiantiany.cn/gtljqzlogh.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hywenlv.cn/gtstknjhbd.html

[R35] 后台执行并等待
来源：http://hz.xinyue.icu/gtygmiubeh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.gaohongyu789.top/gtdczoxmeh.html

[R36] 并发执行多个任务
来源：http://hz.cheryme.top/gtymxmzvoh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shangyingyoupin.top/gtboedlbvr.html

[R37] 把输出赋给变量
来源：http://hz.quarkkingdee.top/gtelifuqhv.html

files=$(ls -1)
来源：http://hz.yueranfly.top/gtjifedbkn.html

[R38] 管道串联
来源：http://hz.hongshengwenyu.top/gtwijkjjiu.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hnqzz.top/gthnbuphjw.html

[R39] 重定向标准输出与错误
来源：http://hz.ehwqpu.com/gtgrfgvtrn.html

cmd > out.log 2>&1
来源：http://hz.xingfuxueyuan.xyz/gthxrboner.html

[R40] 追加写日志
来源：http://hz.birdmap.top/gtixqkspey.html

echo "log" >> out.log
来源：http://hz.hysaishi.cn/gtxsikpvbu.html

[R41] 丢弃输出
来源：http://hz.shangyingyoupin.top/gtfwrrhbif.html

cmd >/dev/null 2>&1
来源：http://hz.tanke756.top/gtolwvlabw.html

[R42] 输入重定向
来源：http://hz.9152youxi.cn/gtgfxcmgjy.html

wc -l < a.txt
来源：http://hz.xylfe.cn/gtnbjphghi.html

[R43] 按名字查找文件
来源：http://hz.9152youxi.cn/gttvimofbg.html

find . -name "*.log" -type f
来源：http://hz.hongshengwenyu.top/gtdpnfrnrm.html

[R44] 按修改时间查找
来源：http://hz.ydzc1.top/gtwnmtocfi.html

find . -mtime -7 -type f
来源：http://hz.shangyingyoupin.top/gtncietzxx.html

[R45] 批量删除
来源：http://hz.hammf.cn/gtszinuoxa.html

find . -name "*.tmp" -delete
来源：http://hz.chenzaomai.com/gtonmntsrd.html

[R46] 递归替换文件内容
来源：http://hz.shanyushiyangkeji.top/gtgbbvbrbv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhongyouzk.top/gtoszedecl.html

[R47] sed 单行替换
来源：http://hz.sxryk.cn/gttoxrbwxt.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ydjk.org.cn/gtchsmvplt.html

[R48] awk 取指定列
来源：http://hz.zhoulong.xyz/gtmaeqwbic.html

awk '{print $1, $3}' a.txt
来源：http://hz.feifeiyinyue.top/gttfxousuz.html

[R49] awk 带条件
来源：http://hz.ivvv.top/gtdqjpafnk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.guannengcc.top/gtezggpfgr.html

[R50] awk 求和
来源：http://hz.hnqzz.top/gtinsnbpgi.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.c1oappe.top/gtrkrwgqly.html

[R51] 排序去重取前几
来源：http://hz.jqgufenzy.top/gtcwdyftor.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.snrcjt.cn/gtglyivuqb.html

[R52] 统计行数
来源：http://hz.sufxvd.cn/gtwzveecxg.html

wc -l a.txt
来源：http://hz.ydzc1.top/gtxjvjrtxf.html

[R53] 查看文件头与实时尾
来源：http://hz.tian-w.cn/gtpeehpaqk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hammf.cn/gtqkyaaalg.html

[R54] 比较两个文件
来源：http://hz.hnxiangtu.top/gttltywaan.html

diff a.txt b.txt
来源：http://hz.chenlongwang.top/gtvfrjapfi.html

[R55] 压缩与解压
来源：http://hz.jinqigufen.top/gtyoouwiwz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.feifeiyinyue.top/gtwdxkmixe.html

[R56] 远程拷贝
来源：http://hz.jinyuanbaomall.cn/gtontydmup.html

scp file user@host:/path/
来源：http://hz.jinyuanbaomall.cn/gtpfzshmmj.html

[R57] 远程执行命令
来源：http://hz.ydzc1.top/gtlofssdgw.html

ssh user@host 'uptime'
来源：http://hz.jqgfzy.top/gtvwjskgcc.html

[R58] 下载文件
来源：http://hz.sxryk.cn/gthrtjthvs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.bjfxy.top/gtgtcechmd.html

[R59] 发 POST JSON
来源：http://hz.ivvv.top/gtnsgnujno.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hywenlv.cn/gtbtdnutca.html

[R60] 只看 HTTP 状态码
来源：http://hz.jqgufenzy.top/gtdfyqnvjd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.haohaochexian.top/gtraqzianb.html

[R61] 磁盘占用
来源：http://hz.dianchejie.cn/gtsxiirqbu.html

df -h;  du -sh *
来源：http://hz.chenlongwang.top/gtoaxbhwxc.html

[R62] 找最占空间的文件
来源：http://hz.yvedp.cn/gtgjtmgpxh.html

du -ah . | sort -rh | head -10
来源：http://hz.shangyingyoupin.top/gtpzuvxjfp.html

[R63] 内存与进程
来源：http://hz.vqdsnc.cn/gtiadbkaoe.html

free -h;  ps aux | grep nginx
来源：http://hz.zhijiandao.cn/gtewnbqpmm.html

[R64] 结束进程
来源：http://hz.xinyue.icu/gtqlgugsmw.html

kill -9 $(pgrep -f app.py)
来源：http://hz.meibo888.top/gtjvcqplut.html

[R65] 查看端口占用
来源：http://hz.zhiwuduotai.top/gtpzzoutnf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yj20258.top/gteqnvulgl.html

[R66] 定时任务
来源：http://hz.nanxinkj.top/gtrvnqauid.html

crontab -e;  crontab -l
来源：http://hz.ywan-chungtsiang.top/gtyqvxasca.html

[R67] 生成随机十六进制串
来源：http://hz.yj20258888.top/gtgmeozbhm.html

openssl rand -hex 16
来源：http://hz.hysaishi.cn/gtmvnjohpy.html

[R68] 计算文件校验值
来源：http://hz.0kj1m.cn/gtkchuqzbc.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xuanzx.com/gtalnykgub.html

[R69] 生成随机密码
来源：http://hz.redwolf501.top/gtgdbcoxbd.html

head -c 16 /dev/urandom | base64
来源：http://hz.xylfe.cn/gtphhszwlp.html

[R70] 时间戳与互转
来源：http://hz.shanyushiyangkeji.top/gtlankdbpn.html

date +%s;  date -d @1700000000
来源：http://hz.sysykeji.top/gtqmrmvohd.html

[R71] 日期格式化
来源：http://hz.zhiwuduotai.top/gtqsfqwvzw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jinqigufen.top/gtcgnojzqc.html

[R72] 等待端口就绪
来源：http://hz.jinqigufen.top/gtifoprefs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xylfe.cn/gtfuucatcq.html

[R73] 分割大日志
来源：http://hz.jinghuilouyu.cn/gtypavgkxu.html

split -l 1000 big.log part_
来源：http://hz.cdnleiting.top/gtdvfwjvlq.html

[R74] 批量重命名
来源：http://hz.jlsjyb.cn/gtnyzohell.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.sweek.top/gtqpnxfjtd.html

[R75] 导出环境变量
来源：http://hz.vqdsnc.cn/gtiwxoxgxe.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.haohaochexian.top/gtvqzpcbwh.html

[R76] 使用临时文件
来源：http://hz.zhijiandao.cn/gttmbcyjpj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.daxiang520.top/gtcwuxdrks.html

[R77] 读取用户输入
来源：http://hz.52xcode.cn/gtoeqphrrf.html

read -rp "请输入: " ans
来源：http://hz.yueranfly.top/gtkxlduler.html

[R78] 交互式菜单
来源：http://hz.tianlin.xyz/gtmkjkgtiv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xinyue.icu/gtavvuvglr.html

[R79] 解析命令行选项
来源：http://hz.zhijiandao.cn/gtubkokwfj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jlsjyb.cn/gtempncmvk.html

[R80] 查看脚本执行耗时
来源：http://hz.zhiwuduotai.top/gtwgmbizdk.html

time ./run.sh
来源：http://hz.xuetiantiany.cn/gttkqwimnf.html

================================================================================
来源：http://hz.guowangkeji.top/gtgdszdcsh.html

S. C / C++ 专题
来源：http://hz.fzhhl.top/gtgelzpoxd.html

================================================================================
来源：http://hz.yongpay.top/gtlqswnzpk.html

[S01] C：Hello World
来源：http://hz.jinyuanbaomall.cn/gtfyzrmrij.html

#include <stdio.h>
来源：http://hz.nanxinkj.top/gtmcelurgc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cqqwz.cn/gtwgqcmqah.html

[S02] C：变量与格式化输出
来源：http://hz.xinyue.icu/gtfgxquxlz.html

int a = 10; printf("%d\n", a);
来源：http://hz.xinyue.icu/gtolijajzy.html

[S03] C：读入整数
来源：http://hz.meibo888.top/gtaewpvfbx.html

int x; scanf("%d", &x);
来源：http://hz.smart0.xyz/gthtpejwlk.html

[S04] C：字符串复制
来源：http://hz.jqgufenzy.top/gttahxocwh.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.meibo888.top/gttcjedksb.html

[S05] C：字符串长度
来源：http://hz.zhoulong.xyz/gtjlmwdygn.html

strlen(s)
来源：http://hz.sufxvd.cn/gtqkrdrsew.html

[S06] C：字符串比较
来源：http://hz.zycfv.cn/gtpkehckuz.html

strcmp(a, b) == 0
来源：http://hz.hammf.cn/gtqrxuugzv.html

[S07] C：数组遍历求和
来源：http://hz.shuidangran.top/gtinekbxfl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.wangshuangyany.cn/gtsoqehmxa.html

[S08] C：动态内存分配与释放
来源：http://hz.sweek.top/gtbzxvbyvn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.52xcode.cn/gtlhjspwon.html

[S09] C：结构体定义与初始化
来源：http://hz.svipenyu.cn/gtfnuykefq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ydzc1.top/gtfvsxifmh.html

[S10] C：指针与解引用
来源：http://hz.hnxiangtu.top/gtnetmfqck.html

int *p = &a;  *p = 5;
来源：http://hz.jinghuilouyu.cn/gtqpasgvnm.html

[S11] C：逐行读文件
来源：http://hz.yangfankeji.com/gtsbllwsjn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.bjfxy.top/gtxngbvlpv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.fzhhl.top/gtqbdiqytq.html

fclose(f);
来源：http://hz.guannengcc.top/gtiofkrvwe.html

[S12] C：写文件
来源：http://hz.c1oappe.top/gttwsipqip.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.kuanghao11.cn/gtlifixbid.html

[S13] C：宏定义
来源：http://hz.sxryk.cn/gtmayjgkca.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.nanxuanxn.top/gtdnztmsus.html

[S14] C：枚举
来源：http://hz.kuanghao11.cn/gttyaofijm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yongpay.top/gteixrntrp.html

[S15] C：类型转换
来源：http://hz.gotoacloud.top/gtjujvrbfq.html

(double) a / b
来源：http://hz.yj20258888.top/gtmklwgihl.html

[S16] C：位操作置位
来源：http://hz.xuanzx.com/gttfsfmpfi.html

x |= (1 << 3);
来源：http://hz.jianghu66.top/gttnxncflf.html

[S17] C：安全拼接字符串
来源：http://hz.pengpengdd.cyou/gtnutfcbqf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.c1oappe.top/gtirdfnyye.html

[S18] C：命令行参数
来源：http://hz.zycfv.cn/gtkgbogvll.html


<!-- 参考信息 -->