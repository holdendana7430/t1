代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.haohaochexian.top/gtrjpznogd.html

[Q50] 批量更新
来源：http://hz.guannengcc.top/gtcyuxovfs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sufxvd.cn/gtniwlwgpa.html

[Q51] 用子查询更新
来源：http://hz.cdnleiting.top/gtihzhclam.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shanyushiyangtech.top/gtmvockflv.html

[Q52] 删除指定行
来源：http://hz.xziqi.cn/gtxkkofumo.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hnqzz.top/gtbxutitrc.html

[Q53] 按条件删除
来源：http://hz.nwbrower.top/gtytrlkvdh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hnqzz.top/gtkroqjwxh.html

[Q54] 清空表
来源：http://hz.jqgfzy.top/gtpzfhhyig.html

TRUNCATE TABLE logs;
来源：http://hz.sufxvd.cn/gtttbrmauh.html

[Q55] 排名（并列占位）
来源：http://hz.sysykeji.top/gtmjakputc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yueranfly.top/gtcftecusi.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yongpay.top/gthxipuqbo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hfpthk.cn/gtidubjvir.html

[Q57] 行号
来源：http://hz.dianchejie.cn/gtpvsinqnh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhoulong.xyz/gtmvsrfowr.html

[Q58] 累计求和
来源：http://hz.zhijiandao.cn/gtzjrhefxn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ybcxt.top/gtqisvkjkt.html

[Q59] 分组内累计
来源：http://hz.jinghuilouyu.cn/gtijusyrxy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xylfe.cn/gtvmspmtet.html

[Q60] 取上一行 / 下一行
来源：http://hz.daria6918.cn/gtstueevpk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shuidangran.top/gtrznpzgok.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gotoacloud.top/gtiuqlwhps.html

[Q61] 移动平均
来源：http://hz.feifeiyinyue.top/gtaikrynpc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.chenlongwang.top/gtnvlhthqo.html

[Q62] 分组占比
来源：http://hz.bjfxy.top/gtbxhxrjea.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hnxiangtu.top/gtjbfespmm.html

[Q63] 开启事务
来源：http://hz.yonumen.top/gthzeywxqp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.sweek.top/gttehlbblh.html

[Q64] 提交事务
来源：http://hz.cashguo.top/gtatlndjzd.html

COMMIT;
来源：http://hz.yj202588.top/gtluklnrqm.html

[Q65] 回滚事务
来源：http://hz.cqqwz.cn/gtoglroazr.html

ROLLBACK;
来源：http://hz.chenjidiqi.icu/gtzwycjjqm.html

[Q66] 行锁查询
来源：http://hz.aizwys.cn/gtqavvsooe.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.andypj.xyz/gtdfonrdvl.html

[Q67] 设置隔离级别
来源：http://hz.yonumen.top/gtqlbhlkgm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jinghuilouyu.cn/gtikfufhih.html

[Q68] 保存点
来源：http://hz.redwolf501.top/gtrgrunscz.html

SAVEPOINT sp1;
来源：http://hz.nanxuanxn.top/gtlwinixwo.html

ROLLBACK TO sp1;
来源：http://hz.zhiwuduotai.top/gtomewqcfk.html

[Q69] 查看执行计划
来源：http://hz.yuanzhike.top/gtwfvxxxao.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.mhx1999.top/gtecnrvffh.html

[Q70] 更新统计信息
来源：http://hz.quarkkingdee.top/gtykglagxl.html

ANALYZE TABLE users;
来源：http://hz.yuanzhike.top/gtnbuwzxru.html

[Q71] 查看建表语句
来源：http://hz.mhx1999.top/gtfutfcqya.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hammf.cn/gtlyibmmog.html

[Q72] 查看索引
来源：http://hz.tanke756.top/gtgmvrvgus.html

SHOW INDEX FROM users;
来源：http://hz.0kj1m.cn/gtzfoyzuxj.html

[Q73] 查看表状态
来源：http://hz.meibo888.top/gtlzpytlso.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yj202588.top/gtqucvaphv.html

[Q74] 强制使用索引
来源：http://hz.zycfv.cn/gtkupktcqt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.c1oappe.top/gtyuricnko.html

[Q75] 日期格式化
来源：http://hz.cqqwz.cn/gtkcaqursu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jinghuilouyu.cn/gtamqsedet.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hongshengwenyu.top/gtbkpsyxnj.html

[Q76] 按天统计
来源：http://hz.zhiwuduotai.top/gtetpesopj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jinqigufen.top/gtvyrgiigc.html

[Q77] 时间加减
来源：http://hz.zycfv.cn/gtuzzkxyst.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.redwolf501.top/gtmmbespbd.html

[Q78] 当前时间
来源：http://hz.havefunace.top/gtdqvfqovc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.bjfxy.top/gtixahaaad.html

[Q79] 字符串拼接
来源：http://hz.tanke756.top/gtiewiyitt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.tianlin.xyz/gtikmlltws.html

[Q80] 字符串截取
来源：http://hz.feifeiyinyue.top/gtsqlnthmy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cashguo.top/gtssobtiij.html

[Q81] 字符串替换
来源：http://hz.chenjidiqi.icu/gtbteewmmf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.fengsongda.top/gtfmwnocxl.html

[Q82] 字符长度与字节长度
来源：http://hz.gaohongyu789.top/gtzprqakal.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.daxiang520.top/gtwypjzlwo.html

[Q83] 大小写转换
来源：http://hz.wangshuangyany.cn/gtwgxukfxb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yongpay.top/gtahcenqbl.html

[Q84] 去除首尾空格
来源：http://hz.gotoacloud.top/gtgqtslprv.html

SELECT TRIM(name) FROM users;
来源：http://hz.iojbl.cn/gticbnwrgk.html

[Q85] 数值取整
来源：http://hz.vqdsnc.cn/gtlzrdhjdz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hnqzz.top/gtpuxxxdyg.html

[Q86] 读取 JSON 字段
来源：http://hz.gogol.net.cn/gtqawpkhhc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.wangdashe.top/gtaithymic.html

[Q87] JSON 字段做条件
来源：http://hz.yongpay.top/gtsapvvqxe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.sysykeji.top/gtcxdtlrfg.html

[Q88] 行转列（条件聚合）
来源：http://hz.ppjwa.cn/gtekepuwyd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.redwolf501.top/gtpilaspyw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.daxiang520.top/gtgevleqga.html

[Q89] 判断表是否存在
来源：http://hz.guannengcc.top/gtimkenxac.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yuanzhike.top/gtymkzvizi.html

[Q90] 生成序号列
来源：http://hz.jqgfzy.top/gtxerdcgrd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.sufxvd.cn/gtfwuftpze.html

================================================================================
来源：http://hz.hnqzz.top/gtnvjuvppl.html

R. Bash 专题
来源：http://hz.vqdsnc.cn/gtxcbpwcap.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtdjlqwuwm.html

[R01] shebang 与严格模式
来源：http://hz.daria6918.cn/gtgonhquec.html

#!/usr/bin/env bash
来源：http://hz.jqgfzy.top/gtzlsvdmow.html

set -euo pipefail
来源：http://hz.sxryk.cn/gthytomqip.html

[R02] 变量赋值与使用
来源：http://hz.gotoacloud.top/gtjutpthik.html

name="Tom"; echo "$name"
来源：http://hz.dianchejie.cn/gtujdyhbgm.html

[R03] 只读变量
来源：http://hz.meibo888.top/gtsqlkkqub.html

readonly PI=3.14
来源：http://hz.hammf.cn/gtamalyvjl.html

[R04] 位置参数
来源：http://hz.dianchejie.cn/gtopeziodo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.sufxvd.cn/gtbebiyjhn.html

[R05] 参数默认值
来源：http://hz.gaohongyu789.top/gttsltzwvr.html

name="${1:-default}"
来源：http://hz.9152youxi.cn/gtizgehlmr.html

[R06] 判断命令是否存在
来源：http://hz.zhiwuduotai.top/gtbjxwjocl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.cheryme.top/gthplkrbmk.html

[R07] if 判断文件
来源：http://hz.vqdsnc.cn/gtiaaugycz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.meibo888.top/gtxgifktkd.html

[R08] 数值比较
来源：http://hz.jinghuilouyu.cn/gtedyiuplk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.smart0.xyz/gtldofykwo.html

[R09] 字符串比较
来源：http://hz.yj202588.top/gtahxpsqzc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jyoumei.cn/gtymmrxzkd.html

[R10] 正则匹配
来源：http://hz.yuxming.cn/gtwtgitgmg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ehwqpu.com/gtwnddcsku.html

[R11] case 多分支
来源：http://hz.mhx1999.top/gtjuqukwyu.html

case "$1" in
来源：http://hz.yongpay.top/gtkizhkdou.html

start) echo "启动" ;;
来源：http://hz.pycfn.com/gtwwqibkpx.html

stop)  echo "停止" ;;
来源：http://hz.shzxlz.cn/gtrkfhriud.html

*)     echo "未知命令" ;;
来源：http://hz.ydjk.org.cn/gtzpmkmxki.html

esac
来源：http://hz.zhiwuduotai.top/gtvlxjalxv.html

[R12] for 遍历文件
来源：http://hz.dashuyun.cn/gtwiswkpue.html

for f in *.txt; do echo "$f"; done
来源：http://hz.52xcode.cn/gtbttjxqzi.html

[R13] for 计数循环
来源：http://hz.xuanzx.com/gtsiqetxsl.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhaomingkeji.xyz/gttajymsvh.html

[R14] C 风格 for
来源：http://hz.hywenlv.cn/gtfzadtxfn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.wangshuangyany.cn/gtfzdoeire.html

[R15] while 逐行读文件
来源：http://hz.cucudq.cn/gtwgioocdg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.redwolf501.top/gtoavraber.html

[R16] until 等待条件
来源：http://hz.guannengcc.top/gtviigodtc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.nanxinkj.top/gtcsfrgayu.html

[R17] 数组定义与取值
来源：http://hz.gzhubu.top/gtaxearcnl.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.316326.xyz/gtvzqhedlv.html

[R18] 遍历数组
来源：http://hz.xuanzx.com/gtperibazm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.316326.xyz/gtrpfslrcf.html

[R19] 数组长度
来源：http://hz.jianghu66.top/gtsrwkhgez.html

echo "${#arr[@]}"
来源：http://hz.havefunace.top/gtzuocfrxv.html

[R20] 关联数组（字典）
来源：http://hz.aizwys.cn/gtcuftnyjz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shanyushiyangtech.top/gtahdsvuse.html

[R21] 字符串长度
来源：http://hz.hongshengwenyu.top/gtlbrxpzcp.html

echo "${#s}"
来源：http://hz.hammf.cn/gthmvurljf.html

[R22] 截取子串
来源：http://hz.hnxiangtu.top/gtcpihwlkk.html

echo "${s:0:5}"
来源：http://hz.zhongyouzk.top/gtgrpyptpq.html

[R23] 字符串替换
来源：http://hz.aizwys.cn/gthdezhxii.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yj20258888.top/gttjlbgfcf.html

[R24] 大小写转换
来源：http://hz.vqdsnc.cn/gtmgsqeruc.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.dashuyun.cn/gtasoiutbp.html

[R25] 去后缀 / 去前缀
来源：http://hz.mhx1999.top/gtwuwoqubb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.mhx1999.top/gtqzxaogfa.html

[R26] 命令替换
来源：http://hz.gotoacloud.top/gtrtzefukh.html

now=$(date +%F); echo "$now"
来源：http://hz.yuxming.cn/gtfkrjinxm.html

[R27] 算术展开
来源：http://hz.vqdsnc.cn/gtfljzrflo.html

echo $((1 + 2 * 3))
来源：http://hz.chenjidiqi.icu/gttupkixsv.html

[R28] 浮点运算
来源：http://hz.ivvv.top/gtmzrqmhdd.html

echo "scale=2; 10/3" | bc
来源：http://hz.jianghu66.top/gteaigcfhz.html

[R29] 定义函数
来源：http://hz.mhx1999.top/gtohuibbmo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.guowangkeji.top/gtuhywwqwk.html

[R30] 函数返回状态码
来源：http://hz.shanyushiyangkeji.top/gtbkobtuuf.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yj20258.top/gtvtgtcglm.html

[R31] 局部变量
来源：http://hz.iojbl.cn/gtcvfxsrvb.html

f() { local x=1; echo "$x"; }
来源：http://hz.jinqigufen.top/gttgjxenqz.html

[R32] 参数个数校验
来源：http://hz.yj202588.top/gtfjlsitpv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jianghu66.top/gtppdabhco.html

[R33] 捕获错误并提示行号
来源：http://hz.jinqigufen.top/gtavyiswbe.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.snrcjt.cn/gtohnddvbv.html

[R34] 退出时清理
来源：http://hz.ivvv.top/gtsfwnelpn.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.pengpengdd.cyou/gtlrqikxyq.html

[R35] 后台执行并等待
来源：http://hz.chenzaomai.com/gtdpnkkkbi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.daria6918.cn/gtqppstatn.html

[R36] 并发执行多个任务
来源：http://hz.zhiwuduotai.top/gtkellajqn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.iojbl.cn/gtrkvomvnq.html

[R37] 把输出赋给变量
来源：http://hz.ybcxt.top/gtwvozkias.html

files=$(ls -1)
来源：http://hz.jqgfzy.top/gtxkclfnzz.html

[R38] 管道串联
来源：http://hz.wangshuangyany.cn/gthulvyslr.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yj20258.top/gtcommzvxr.html

[R39] 重定向标准输出与错误
来源：http://hz.guowangkeji.top/gtibfimxvp.html

cmd > out.log 2>&1
来源：http://hz.yj202588.top/gtfbvkmpfm.html

[R40] 追加写日志
来源：http://hz.zycfv.cn/gtnojgarmp.html

echo "log" >> out.log
来源：http://hz.fengsongda.top/gtlsupgpcy.html

[R41] 丢弃输出
来源：http://hz.wangshuangyany.cn/gtvgvigedw.html

cmd >/dev/null 2>&1
来源：http://hz.yj20258.top/gtnqqcmzgo.html

[R42] 输入重定向
来源：http://hz.xingfuxueyuan.xyz/gtqgttfkvc.html

wc -l < a.txt
来源：http://hz.zhijiandao.cn/gtncltkyjy.html

[R43] 按名字查找文件
来源：http://hz.jlsjyb.cn/gtaiixkygt.html

find . -name "*.log" -type f
来源：http://hz.hysaishi.cn/gtkiiswwil.html

[R44] 按修改时间查找
来源：http://hz.yuanzhike.top/gtmrnjbego.html

find . -mtime -7 -type f
来源：http://hz.pengpengdd.cyou/gtmeduhxyw.html

[R45] 批量删除
来源：http://hz.hnxiangtu.top/gtxedfbbcs.html

find . -name "*.tmp" -delete
来源：http://hz.aizwys.cn/gtxgcfdqzs.html

[R46] 递归替换文件内容
来源：http://hz.smart0.xyz/gtbeictflx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jinqigfzy.top/gtagvabzvd.html

[R47] sed 单行替换
来源：http://hz.yueranfly.top/gtkvnhmdns.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hnqzz.top/gtmlrizgqu.html

[R48] awk 取指定列
来源：http://hz.wangshuangyany.cn/gtqgkmfwgj.html

awk '{print $1, $3}' a.txt
来源：http://hz.birdmap.top/gtrbitpcmp.html

[R49] awk 带条件
来源：http://hz.xuanzx.com/gtsairbwhu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xuanzx.com/gtwxhdvnha.html

[R50] awk 求和
来源：http://hz.gogol.net.cn/gtgjyinokt.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hfpthk.cn/gtsqulwgby.html

[R51] 排序去重取前几
来源：http://hz.redwolf501.top/gtpfauksxd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhixingplan.top/gtmemwnhou.html

[R52] 统计行数
来源：http://hz.gaohongyu789.top/gtywpbancd.html

wc -l a.txt
来源：http://hz.jinyuanbaomall.cn/gtpckpnnji.html

[R53] 查看文件头与实时尾
来源：http://hz.nanxuanxn.top/gtsqbwvfpw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.daria6918.cn/gtkogzpfca.html

[R54] 比较两个文件
来源：http://hz.fengsongda.top/gtjmytbldh.html

diff a.txt b.txt
来源：http://hz.chenlongwang.top/gtiersbogd.html

[R55] 压缩与解压
来源：http://hz.jyoumei.cn/gtgaazgbkz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.vqdsnc.cn/gtaqwyfqtu.html

[R56] 远程拷贝
来源：http://hz.52xcode.cn/gttirxerhg.html

scp file user@host:/path/
来源：http://hz.gaohongyu789.top/gtcyjxibbb.html

[R57] 远程执行命令
来源：http://hz.zycfv.cn/gtqqmttzfb.html

ssh user@host 'uptime'
来源：http://hz.vqdsnc.cn/gtlcgbcuuc.html

[R58] 下载文件
来源：http://hz.yonumen.top/gtpvstlqxn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.sysykeji.top/gtcukjuqpe.html

[R59] 发 POST JSON
来源：http://hz.chenlongwang.top/gtfzxxkztc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.tian-w.cn/gtmelbzrtz.html

[R60] 只看 HTTP 状态码
来源：http://hz.hysaishi.cn/gteyxncbfu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xingfuxueyuan.xyz/gtovgbyrpr.html

[R61] 磁盘占用
来源：http://hz.andypj.xyz/gtefysmihx.html

df -h;  du -sh *
来源：http://hz.xinyue.icu/gtfrybirom.html

[R62] 找最占空间的文件
来源：http://hz.hnxiangtu.top/gtzlxypegv.html

du -ah . | sort -rh | head -10
来源：http://hz.fzhhl.top/gtnlvvdhuo.html

[R63] 内存与进程
来源：http://hz.pycfn.com/gtvomuczja.html

free -h;  ps aux | grep nginx
来源：http://hz.yj20258888.top/gtjiwajwbg.html

[R64] 结束进程
来源：http://hz.jqgfzy.top/gtkkeybzgq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.birdmap.top/gtdhxlzojk.html

[R65] 查看端口占用
来源：http://hz.chenlongwang.top/gtanmxfdqm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jinghuilouyu.cn/gtqlcjmfud.html

[R66] 定时任务
来源：http://hz.sweek.top/gtgbipfhvt.html

crontab -e;  crontab -l
来源：http://hz.haohaochexian.top/gtvudvuqcd.html

[R67] 生成随机十六进制串
来源：http://hz.pycfn.com/gtqlyhmejt.html

openssl rand -hex 16
来源：http://hz.ydjk.org.cn/gtsadzjnyq.html

[R68] 计算文件校验值
来源：http://hz.jianghu66.top/gtrcnnzlht.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jianghu66.top/gtcddkvese.html

[R69] 生成随机密码
来源：http://hz.ivvv.top/gtdvnelqql.html

head -c 16 /dev/urandom | base64
来源：http://hz.gaohongyu789.top/gtemtcngzw.html

[R70] 时间戳与互转
来源：http://hz.ydjk.org.cn/gtsguefeoh.html

date +%s;  date -d @1700000000
来源：http://hz.shuidangran.top/gtrnvuduxz.html

[R71] 日期格式化
来源：http://hz.zhiwuduotai.top/gtbwfkfisp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.chenzaomai.com/gthofkurzt.html

[R72] 等待端口就绪
来源：http://hz.c1oappe.top/gtjreblyle.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jqgfzy.top/gtaihmbhtj.html

[R73] 分割大日志
来源：http://hz.nwbrower.top/gtrecjswtl.html

split -l 1000 big.log part_
来源：http://hz.yueranfly.top/gtlcqzwhba.html

[R74] 批量重命名
来源：http://hz.xingfuxueyuan.xyz/gtbvcijonk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhongyouzk.top/gtvwatjtmi.html

[R75] 导出环境变量
来源：http://hz.ehwqpu.com/gtbybqsqgq.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yuxming.cn/gtjlbfcxcp.html

[R76] 使用临时文件
来源：http://hz.ivvv.top/gthnckvsrn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.fengsongda.top/gtnxoyqgrm.html

[R77] 读取用户输入
来源：http://hz.gogol.net.cn/gtqhqvvgzd.html

read -rp "请输入: " ans
来源：http://hz.mhx1999.top/gtkuspqhtl.html

[R78] 交互式菜单
来源：http://hz.redwolf501.top/gtsyxwgdtv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jqgufenzy.top/gtpuuxbgor.html

[R79] 解析命令行选项
来源：http://hz.yueranfly.top/gtvtdothue.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cashguo.top/gtmokenvlq.html

[R80] 查看脚本执行耗时
来源：http://hz.jianghu66.top/gtrqboavbw.html

time ./run.sh
来源：http://hz.hfpthk.cn/gtwfrggytc.html

================================================================================
来源：http://hz.tanke756.top/gtyluadqcn.html

S. C / C++ 专题
来源：http://hz.shanyushiyangkeji.top/gtkbcgwczl.html

================================================================================
来源：http://hz.cqqwz.cn/gtqlvghfsy.html

[S01] C：Hello World
来源：http://hz.yanxiufei.cn/gtkcnnhbls.html

#include <stdio.h>
来源：http://hz.hysaishi.cn/gtnslmnarp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cqqwz.cn/gtginoaidj.html

[S02] C：变量与格式化输出
来源：http://hz.svipenyu.cn/gtltojcsqw.html

int a = 10; printf("%d\n", a);
来源：http://hz.yj202588.top/gtyrkxfeal.html

[S03] C：读入整数
来源：http://hz.xylfe.cn/gtyuygpojz.html

int x; scanf("%d", &x);
来源：http://hz.jyoumei.cn/gtltkzkuqc.html

[S04] C：字符串复制
来源：http://hz.cqqwz.cn/gtyuducoct.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xinyue.icu/gtgghihqfl.html

[S05] C：字符串长度
来源：http://hz.birdmap.top/gtamfxcehl.html

strlen(s)
来源：http://hz.vqdsnc.cn/gtxfhxgvrh.html

[S06] C：字符串比较
来源：http://hz.feifeiyinyue.top/gtrulvqofr.html

strcmp(a, b) == 0
来源：http://hz.dianchejie.cn/gtturhyjml.html

[S07] C：数组遍历求和
来源：http://hz.xingfuxueyuan.xyz/gtuficszbu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.wangdashe.top/gtzqamlimi.html

[S08] C：动态内存分配与释放
来源：http://hz.hfpthk.cn/gtyjamphnr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hysaishi.cn/gtgchioysd.html

[S09] C：结构体定义与初始化
来源：http://hz.zhiwuduotai.top/gtcinmaftq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.sweek.top/gtrumgguve.html

[S10] C：指针与解引用
来源：http://hz.xuanzx.com/gtnxfxzxdw.html

int *p = &a;  *p = 5;
来源：http://hz.zhijiandao.cn/gtretwgoot.html

[S11] C：逐行读文件
来源：http://hz.kuanghao11.cn/gtgnoriwxv.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yongpay.top/gthhupamdj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jiagoushi.top/gtxxczlzjz.html

fclose(f);
来源：http://hz.feifeiyinyue.top/gtaargpdxf.html

[S12] C：写文件
来源：http://hz.iojbl.cn/gtedvzxyur.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.dianchejie.cn/gtgcpjbvqe.html

[S13] C：宏定义
来源：http://hz.shuidangran.top/gtboisizzk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.chenlongwang.top/gtwqwgcive.html

[S14] C：枚举
来源：http://hz.jyoumei.cn/gtiazvenul.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xziqi.cn/gtkuugetae.html

[S15] C：类型转换
来源：http://hz.sweek.top/gttimoggsc.html

(double) a / b
来源：http://hz.ydzc1.top/gtdtjaxzon.html

[S16] C：位操作置位
来源：http://hz.cucudq.cn/gtzrwbydxb.html

x |= (1 << 3);
来源：http://hz.jyoumei.cn/gtxmojldcz.html

[S17] C：安全拼接字符串
来源：http://hz.cqqwz.cn/gtsokzynek.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yuxming.cn/gtyncvineq.html

[S18] C：命令行参数
来源：http://hz.hfpthk.cn/gtavbtfcel.html

int main(int argc, char **argv)
来源：http://hz.hysaishi.cn/gtsnrfkmmk.html

[S19] C：快速排序
来源：http://hz.zhengqikj.top/gtrqefvdro.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jinyuanbaomall.cn/gtviomqvdl.html

[S20] C：二分查找
来源：http://hz.jqgfzy.top/gteaywinxz.html


<!-- 参考信息 -->