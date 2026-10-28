代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.bjfxy.top/gtcutkdcfw.html

[Q56] 密集排名（并列不占位）
来源：http://hz.fengsongda.top/gtximdjgpo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.aibaodan.cn/gtxwabzmwb.html

[Q57] 行号
来源：http://hz.zhengqikj.top/gtgnyxnnse.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cashguo.top/gtcwpknhew.html

[Q58] 累计求和
来源：http://hz.cqqwz.cn/gtehqnhpxn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.havefunace.top/gtcnpxmkyp.html

[Q59] 分组内累计
来源：http://hz.nanxuanxn.top/gtbsrlnajj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhixingplan.top/gtnshipekf.html

[Q60] 取上一行 / 下一行
来源：http://hz.snrcjt.cn/gtnfgjfuxe.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jqgufenzy.top/gtfdwybelu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.haohaochexian.top/gtmbnbilyw.html

[Q61] 移动平均
来源：http://hz.jinqigfzy.top/gturlhewiv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yangfankeji.com/gtxlpmjvkb.html

[Q62] 分组占比
来源：http://hz.tian-w.cn/gtjrwrgnud.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.redwolf501.top/gtdyoiquqy.html

[Q63] 开启事务
来源：http://hz.chenlongwang.top/gtefkdjgrr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hammf.cn/gtxpjqeucu.html

[Q64] 提交事务
来源：http://hz.yanxiufei.cn/gtondcocmj.html

COMMIT;
来源：http://hz.smart0.xyz/gtqzbngpex.html

[Q65] 回滚事务
来源：http://hz.sxryk.cn/gtsmafpkta.html

ROLLBACK;
来源：http://hz.svipenyu.cn/gtkxyhzvsg.html

[Q66] 行锁查询
来源：http://hz.tian-w.cn/gtaufayfdg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jinyuanbaomall.cn/gtcmipiamb.html

[Q67] 设置隔离级别
来源：http://hz.tian-w.cn/gttwjeeafm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jiagoushi.top/gttebgspiu.html

[Q68] 保存点
来源：http://hz.cqqwz.cn/gtbyrjtkxe.html

SAVEPOINT sp1;
来源：http://hz.andypj.xyz/gtwuxzgokf.html

ROLLBACK TO sp1;
来源：http://hz.xuetiantiany.cn/gtphihqxct.html

[Q69] 查看执行计划
来源：http://hz.cucudq.cn/gtfybmbiwj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhongyouzk.top/gtbhpgxjis.html

[Q70] 更新统计信息
来源：http://hz.xinyue.icu/gtjvyrsxkl.html

ANALYZE TABLE users;
来源：http://hz.kuanghao11.cn/gtpdwkszic.html

[Q71] 查看建表语句
来源：http://hz.dianchejie.cn/gtdwtszrpj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xziqi.cn/gtzmwgwngs.html

[Q72] 查看索引
来源：http://hz.gotoacloud.top/gtilwwiejw.html

SHOW INDEX FROM users;
来源：http://hz.cashguo.top/gtpakyfpzv.html

[Q73] 查看表状态
来源：http://hz.shuidangran.top/gtndzutyof.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.nanxuanxn.top/gthwapnhjt.html

[Q74] 强制使用索引
来源：http://hz.jinqigufen.top/gttloqzatv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yonumen.top/gtfkvaxcwn.html

[Q75] 日期格式化
来源：http://hz.wangdashe.top/gtlqfryidj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cqqwz.cn/gtsbgosmew.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yvedp.cn/gtjjysecxr.html

[Q76] 按天统计
来源：http://hz.smart0.xyz/gtknefhkpd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shanyushiyangtech.top/gtozxxoevi.html

[Q77] 时间加减
来源：http://hz.mhx1999.top/gthxtbpfpx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jyoumei.cn/gtjsqjvkka.html

[Q78] 当前时间
来源：http://hz.sysykeji.top/gtznedhart.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.chenjidiqi.icu/gtvbkwnyma.html

[Q79] 字符串拼接
来源：http://hz.wangdashe.top/gtvlkhtgbm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.aibaodan.cn/gtxjthscdu.html

[Q80] 字符串截取
来源：http://hz.daxiang520.top/gttucuoeqh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xziqi.cn/gtaifsufxk.html

[Q81] 字符串替换
来源：http://hz.zhaomingkeji.xyz/gtxcftxige.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.aibaodan.cn/gtcppoaksb.html

[Q82] 字符长度与字节长度
来源：http://hz.52xcode.cn/gtvrzsplva.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhoulong.xyz/gtqremlulf.html

[Q83] 大小写转换
来源：http://hz.jinyuanbaomall.cn/gtzmojhhjx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cdnleiting.top/gtahfdtkjk.html

[Q84] 去除首尾空格
来源：http://hz.cucudq.cn/gttpbuqciw.html

SELECT TRIM(name) FROM users;
来源：http://hz.hywenlv.cn/gtzbrctoks.html

[Q85] 数值取整
来源：http://hz.hnqzz.top/gtlihrvcwr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yj20258.top/gtlhdarogo.html

[Q86] 读取 JSON 字段
来源：http://hz.smart0.xyz/gtjtarawde.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.shzxlz.cn/gtfhruayfu.html

[Q87] JSON 字段做条件
来源：http://hz.ivvv.top/gtsifjzjxc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cqqwz.cn/gtkuwuhkcl.html

[Q88] 行转列（条件聚合）
来源：http://hz.xinyue.icu/gtserdmido.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.aibaodan.cn/gtpizcksem.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.gotoacloud.top/gtxiwzwzkd.html

[Q89] 判断表是否存在
来源：http://hz.kuanghao11.cn/gtxpjznoby.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.sufxvd.cn/gtfejtjisg.html

[Q90] 生成序号列
来源：http://hz.zhixingplan.top/gtjivuafbj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.gzhubu.top/gtvculopny.html

================================================================================
来源：http://hz.cqqwz.cn/gtydlencip.html

R. Bash 专题
来源：http://hz.yangfankeji.com/gtyqpdfbgn.html

================================================================================
来源：http://hz.cucudq.cn/gtrekzzzzq.html

[R01] shebang 与严格模式
来源：http://hz.kuanghao11.cn/gtozbagodz.html

#!/usr/bin/env bash
来源：http://hz.zhengqikj.top/gtdnptcypc.html

set -euo pipefail
来源：http://hz.redwolf501.top/gtkbhxtzfv.html

[R02] 变量赋值与使用
来源：http://hz.zhengqikj.top/gtpmpungrx.html

name="Tom"; echo "$name"
来源：http://hz.hammf.cn/gtipofaycz.html

[R03] 只读变量
来源：http://hz.xziqi.cn/gtsibyykpy.html

readonly PI=3.14
来源：http://hz.ppjwa.cn/gttlrzljvp.html

[R04] 位置参数
来源：http://hz.wangshuangyany.cn/gtbhegkmue.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhoulong.xyz/gtsimrdoyb.html

[R05] 参数默认值
来源：http://hz.yvedp.cn/gtjkttdote.html

name="${1:-default}"
来源：http://hz.shuidangran.top/gtpwhawpsi.html

[R06] 判断命令是否存在
来源：http://hz.chenzaomai.com/gtnooxqaqr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ehwqpu.com/gtthrqvzgg.html

[R07] if 判断文件
来源：http://hz.jinghuilouyu.cn/gtlogukgim.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yj202588.top/gtvgxbwwwl.html

[R08] 数值比较
来源：http://hz.zhijiandao.cn/gtypwwduef.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.sweek.top/gtqqgpdmvi.html

[R09] 字符串比较
来源：http://hz.havefunace.top/gtttejyvnf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yangfankeji.com/gtcvaifkxm.html

[R10] 正则匹配
来源：http://hz.zhongyouzk.top/gtwlydrurj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.pengpengdd.cyou/gttvtpllqh.html

[R11] case 多分支
来源：http://hz.birdmap.top/gtxepbcczt.html

case "$1" in
来源：http://hz.52xcode.cn/gtkxwijawo.html

start) echo "启动" ;;
来源：http://hz.jlsjyb.cn/gtfuqgoncg.html

stop)  echo "停止" ;;
来源：http://hz.haohaochexian.top/gtbapjiipm.html

*)     echo "未知命令" ;;
来源：http://hz.jiagoushi.top/gtskcpmnij.html

esac
来源：http://hz.hnqzz.top/gtmlnlnwjg.html

[R12] for 遍历文件
来源：http://hz.0kj1m.cn/gttxrskaxz.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cqqwz.cn/gtzarjiyjo.html

[R13] for 计数循环
来源：http://hz.gotoacloud.top/gtjwbqmjrd.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.pycfn.com/gtyfhoybwx.html

[R14] C 风格 for
来源：http://hz.pycfn.com/gttplblqwj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.nanxinkj.top/gtubkqlstw.html

[R15] while 逐行读文件
来源：http://hz.sxryk.cn/gtngvswmzy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.bjfxy.top/gtuwnzofjy.html

[R16] until 等待条件
来源：http://hz.sxryk.cn/gtkorwdlhx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ybcxt.top/gtxvmpeokq.html

[R17] 数组定义与取值
来源：http://hz.haohaochexian.top/gtvmqgools.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ivvv.top/gtkprgvfqu.html

[R18] 遍历数组
来源：http://hz.jinqigufen.top/gtszwghnah.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xuetiantiany.cn/gtslbwbzrp.html

[R19] 数组长度
来源：http://hz.cucudq.cn/gtzgfcxpwz.html

echo "${#arr[@]}"
来源：http://hz.meibo888.top/gttxswarsq.html

[R20] 关联数组（字典）
来源：http://hz.aibaodan.cn/gtjfqshgep.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jyoumei.cn/gtamnkajfu.html

[R21] 字符串长度
来源：http://hz.jinyuanbaomall.cn/gteftkidax.html

echo "${#s}"
来源：http://hz.sweek.top/gtsctxggep.html

[R22] 截取子串
来源：http://hz.havefunace.top/gtejjnegex.html

echo "${s:0:5}"
来源：http://hz.gogol.net.cn/gteaodcrcf.html

[R23] 字符串替换
来源：http://hz.shanyushiyangkeji.top/gtqcocoyzn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yuxming.cn/gtaxgyjhlp.html

[R24] 大小写转换
来源：http://hz.ppjwa.cn/gtozlwubfu.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.gzhubu.top/gtrwakxeof.html

[R25] 去后缀 / 去前缀
来源：http://hz.fengsongda.top/gtzacelucx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.52xcode.cn/gtpzvigpvk.html

[R26] 命令替换
来源：http://hz.pycfn.com/gtleyzhfha.html

now=$(date +%F); echo "$now"
来源：http://hz.shanyushiyangtech.top/gtlzktxjtm.html

[R27] 算术展开
来源：http://hz.zhiwuduotai.top/gtqgvigwkc.html

echo $((1 + 2 * 3))
来源：http://hz.tianlin.xyz/gtfrqcfege.html

[R28] 浮点运算
来源：http://hz.gotoacloud.top/gtzzcstkfp.html

echo "scale=2; 10/3" | bc
来源：http://hz.cucudq.cn/gtvlrzafzp.html

[R29] 定义函数
来源：http://hz.wangdashe.top/gtzfhuvymy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yj20258888.top/gtmowbdfqs.html

[R30] 函数返回状态码
来源：http://hz.sweek.top/gtmtqgvdof.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hnqzz.top/gtctzunust.html

[R31] 局部变量
来源：http://hz.cdnleiting.top/gtnvsqcjer.html

f() { local x=1; echo "$x"; }
来源：http://hz.shzxlz.cn/gtmtuzavjl.html

[R32] 参数个数校验
来源：http://hz.yonumen.top/gtoqskjbai.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.dashuyun.cn/gtjvibrslj.html

[R33] 捕获错误并提示行号
来源：http://hz.redwolf501.top/gtgrugyydh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jyoumei.cn/gtexqrhmna.html

[R34] 退出时清理
来源：http://hz.ydzc1.top/gtvomzfgxo.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ivvv.top/gtkawkyqck.html

[R35] 后台执行并等待
来源：http://hz.zdqjudy.top/gtwnfxpmon.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.nanxuanxn.top/gtfsoxwifw.html

[R36] 并发执行多个任务
来源：http://hz.ehwqpu.com/gtuxiujvrd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yonumen.top/gtgoqvjbmw.html

[R37] 把输出赋给变量
来源：http://hz.shanyushiyangtech.top/gtwspivgvz.html

files=$(ls -1)
来源：http://hz.cashguo.top/gtuehfttae.html

[R38] 管道串联
来源：http://hz.fzhhl.top/gtmhzmltpr.html

cat a.txt | grep -i error | wc -l
来源：http://hz.gogol.net.cn/gtarvqbyoy.html

[R39] 重定向标准输出与错误
来源：http://hz.jlsjyb.cn/gtctyrhsht.html

cmd > out.log 2>&1
来源：http://hz.sxryk.cn/gtnicapbma.html

[R40] 追加写日志
来源：http://hz.dianchejie.cn/gtbvbpfikl.html

echo "log" >> out.log
来源：http://hz.kuanghao11.cn/gtpzzmgoik.html

[R41] 丢弃输出
来源：http://hz.birdmap.top/gtninalefq.html

cmd >/dev/null 2>&1
来源：http://hz.shangyingyoupin.top/gtamdpxknl.html

[R42] 输入重定向
来源：http://hz.hongshengwenyu.top/gtrpjqgjon.html

wc -l < a.txt
来源：http://hz.quarkkingdee.top/gtnbprfyju.html

[R43] 按名字查找文件
来源：http://hz.sweek.top/gtsvavatit.html

find . -name "*.log" -type f
来源：http://hz.jinyuanbaomall.cn/gtzoickfre.html

[R44] 按修改时间查找
来源：http://hz.shanyushiyangtech.top/gtrmxkyecx.html

find . -mtime -7 -type f
来源：http://hz.iojbl.cn/gtoecvmmio.html

[R45] 批量删除
来源：http://hz.wangdashe.top/gtagdxyqxf.html

find . -name "*.tmp" -delete
来源：http://hz.fengsongda.top/gtegpdjbor.html

[R46] 递归替换文件内容
来源：http://hz.jyoumei.cn/gttxyualcw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.mhx1999.top/gtdhzpxvyj.html

[R47] sed 单行替换
来源：http://hz.hnxiangtu.top/gtewyekpsh.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.wangdashe.top/gtzhttqbth.html

[R48] awk 取指定列
来源：http://hz.svipenyu.cn/gtgocjtgvw.html

awk '{print $1, $3}' a.txt
来源：http://hz.birdmap.top/gtclaehnpe.html

[R49] awk 带条件
来源：http://hz.sufxvd.cn/gtinrkvkng.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xuanzx.com/gtzmkmlpuw.html

[R50] awk 求和
来源：http://hz.yonumen.top/gtrrcetnxe.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.aibaodan.cn/gtrldvasxg.html

[R51] 排序去重取前几
来源：http://hz.haohaochexian.top/gtkfzmdnvv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gzhubu.top/gtzgmjtjjb.html

[R52] 统计行数
来源：http://hz.dashuyun.cn/gtluvgnnvt.html

wc -l a.txt
来源：http://hz.ppjwa.cn/gtwnqbsbhd.html

[R53] 查看文件头与实时尾
来源：http://hz.gzhubu.top/gtzzjwpwii.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jinqigufen.top/gthkwdcxku.html

[R54] 比较两个文件
来源：http://hz.shzxlz.cn/gtmbjrnnzo.html

diff a.txt b.txt
来源：http://hz.snrcjt.cn/gtgbbjtidl.html

[R55] 压缩与解压
来源：http://hz.sweek.top/gtdnbgqfqd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.havefunace.top/gthianxnnf.html

[R56] 远程拷贝
来源：http://hz.chenzaomai.com/gtmlahknna.html

scp file user@host:/path/
来源：http://hz.sufxvd.cn/gtzcznhxih.html

[R57] 远程执行命令
来源：http://hz.pycfn.com/gtrezykonr.html

ssh user@host 'uptime'
来源：http://hz.c1oappe.top/gtyznpfzbh.html

[R58] 下载文件
来源：http://hz.pycfn.com/gttecjorqe.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhoulong.xyz/gtlawrxyyi.html

[R59] 发 POST JSON
来源：http://hz.hongshengwenyu.top/gtaqszebuo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.wangdashe.top/gtckmgkqyx.html

[R60] 只看 HTTP 状态码
来源：http://hz.gzhubu.top/gtobzlsfdw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ehwqpu.com/gtvlmeddsh.html

[R61] 磁盘占用
来源：http://hz.quarkkingdee.top/gtdlrgawyf.html

df -h;  du -sh *
来源：http://hz.hywenlv.cn/gthcufwunk.html

[R62] 找最占空间的文件
来源：http://hz.daria6918.cn/gtoacofasq.html

du -ah . | sort -rh | head -10
来源：http://hz.daxiang520.top/gtvlurivzc.html

[R63] 内存与进程
来源：http://hz.yonumen.top/gtxxtkovyl.html

free -h;  ps aux | grep nginx
来源：http://hz.jqgfzy.top/gtbfbvuhzh.html

[R64] 结束进程
来源：http://hz.nanxinkj.top/gtgijimljt.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yj20258.top/gtnftjukip.html

[R65] 查看端口占用
来源：http://hz.sufxvd.cn/gtuhaohxtp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xuetiantiany.cn/gtchiunciw.html

[R66] 定时任务
来源：http://hz.xuetiantiany.cn/gtfsmttvly.html

crontab -e;  crontab -l
来源：http://hz.sysykeji.top/gtsfsimjij.html

[R67] 生成随机十六进制串
来源：http://hz.jinqigufen.top/gtreaphboz.html

openssl rand -hex 16
来源：http://hz.dashuyun.cn/gtvqybebog.html

[R68] 计算文件校验值
来源：http://hz.nanxinkj.top/gtkkywyrtz.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.feifeiyinyue.top/gtqvdzczws.html

[R69] 生成随机密码
来源：http://hz.ydjk.org.cn/gtiatzbvnp.html

head -c 16 /dev/urandom | base64
来源：http://hz.jianghu66.top/gtebtxsecg.html

[R70] 时间戳与互转
来源：http://hz.yuanzhike.top/gthkumubtd.html

date +%s;  date -d @1700000000
来源：http://hz.pengpengdd.cyou/gteganejtz.html

[R71] 日期格式化
来源：http://hz.jqgufenzy.top/gtvragkmjt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.feifeiyinyue.top/gtxakioqwx.html

[R72] 等待端口就绪
来源：http://hz.snrcjt.cn/gttoeckvof.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.pycfn.com/gtjapfwmhs.html

[R73] 分割大日志
来源：http://hz.dashuyun.cn/gtrnbdmbta.html

split -l 1000 big.log part_
来源：http://hz.cucudq.cn/gtnqopjuty.html

[R74] 批量重命名
来源：http://hz.smart0.xyz/gtyacmqvez.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shanyushiyangtech.top/gtubjwadxg.html

[R75] 导出环境变量
来源：http://hz.nwbrower.top/gtgrihbico.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ivvv.top/gtdpddmyor.html

[R76] 使用临时文件
来源：http://hz.xylfe.cn/gtyeqeztxz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.daria6918.cn/gtvscjhxxe.html

[R77] 读取用户输入
来源：http://hz.xingfuxueyuan.xyz/gtdahrdzts.html

read -rp "请输入: " ans
来源：http://hz.fzhhl.top/gtqwgnnuuq.html

[R78] 交互式菜单
来源：http://hz.gogol.net.cn/gtlxgvcdjd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.haohaochexian.top/gtuorfcmsr.html

[R79] 解析命令行选项
来源：http://hz.chenzaomai.com/gtqvjkmwmg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhaomingkeji.xyz/gtilhxyjrl.html

[R80] 查看脚本执行耗时
来源：http://hz.shangyingyoupin.top/gtanwnntjj.html

time ./run.sh
来源：http://hz.feifeiyinyue.top/gteoamokqb.html

================================================================================
来源：http://hz.yuxming.cn/gtbtbmhfsb.html

S. C / C++ 专题
来源：http://hz.yj202588.top/gtpddrveam.html

================================================================================
来源：http://hz.yj202588.top/gtxbfdmvov.html

[S01] C：Hello World
来源：http://hz.jinyuanbaomall.cn/gtkllsvnng.html

#include <stdio.h>
来源：http://hz.cucudq.cn/gtibgnwpld.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ehwqpu.com/gtollblkwu.html

[S02] C：变量与格式化输出
来源：http://hz.wangdashe.top/gtxcwzbwjw.html

int a = 10; printf("%d\n", a);
来源：http://hz.52xcode.cn/gtixpqrvyw.html

[S03] C：读入整数
来源：http://hz.zycfv.cn/gtxmkuoyez.html

int x; scanf("%d", &x);
来源：http://hz.cdnleiting.top/gtczrqdqwn.html

[S04] C：字符串复制
来源：http://hz.havefunace.top/gtqtcfnhem.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.iojbl.cn/gtasjkvrpz.html

[S05] C：字符串长度
来源：http://hz.ppjwa.cn/gtlzmuipao.html

strlen(s)
来源：http://hz.sufxvd.cn/gtbbbfnzqe.html

[S06] C：字符串比较
来源：http://hz.cdnleiting.top/gtebojabfe.html

strcmp(a, b) == 0
来源：http://hz.dashuyun.cn/gtexgyjsla.html

[S07] C：数组遍历求和
来源：http://hz.tian-w.cn/gtvoqjggxi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.wangdashe.top/gtidvrzhwq.html

[S08] C：动态内存分配与释放
来源：http://hz.jqgufenzy.top/gtenmecenn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinqigufen.top/gtqitwxmoj.html

[S09] C：结构体定义与初始化
来源：http://hz.zhaomingkeji.xyz/gtfztnlkyy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xziqi.cn/gtbgxxrenw.html

[S10] C：指针与解引用
来源：http://hz.tanke756.top/gthaxxomzj.html

int *p = &a;  *p = 5;
来源：http://hz.jianghu66.top/gtqdhljonm.html

[S11] C：逐行读文件
来源：http://hz.shangyingyoupin.top/gtzuicnqcs.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.tian-w.cn/gtxnveyrxz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nwbrower.top/gtytpnffqb.html

fclose(f);
来源：http://hz.zhaomingkeji.xyz/gtmixucifw.html

[S12] C：写文件
来源：http://hz.hongshengwenyu.top/gtgzpslbbs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gzhubu.top/gtetzmtjxo.html

[S13] C：宏定义
来源：http://hz.52xcode.cn/gtyknhiron.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yj202588.top/gtardnmzwx.html

[S14] C：枚举
来源：http://hz.pycfn.com/gtwwbockip.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yongpay.top/gtzstjgnfo.html

[S15] C：类型转换
来源：http://hz.daxiang520.top/gthogwgliy.html

(double) a / b
来源：http://hz.meibo888.top/gtwuzypxsq.html

[S16] C：位操作置位
来源：http://hz.redwolf501.top/gtgrjerweh.html

x |= (1 << 3);
来源：http://hz.cqqwz.cn/gtqhewiiwe.html

[S17] C：安全拼接字符串
来源：http://hz.xuanzx.com/gtkhrgukfy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cdnleiting.top/gtunhsvtsh.html

[S18] C：命令行参数
来源：http://hz.shuidangran.top/gtxqzfyyhu.html

int main(int argc, char **argv)
来源：http://hz.daria6918.cn/gtvyvxjvci.html

[S19] C：快速排序
来源：http://hz.havefunace.top/gtphoxwagn.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.0kj1m.cn/gtjbrxhrll.html

[S20] C：二分查找
来源：http://hz.jyoumei.cn/gtszboonjv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jinghuilouyu.cn/gtoqjiukpo.html

[S21] C：字符类别判断
来源：http://hz.9152youxi.cn/gtzkyjplof.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhixingplan.top/gttwyxefrl.html

[S22] C：字符串转数字
来源：http://hz.zhijiandao.cn/gtzpbyrsks.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhengqikj.top/gtnwvldvku.html

[S23] C：随机数
来源：http://hz.zhoulong.xyz/gtmcdgcxet.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.quarkkingdee.top/gtklhsxbog.html

[S24] C：获取本地时间
来源：http://hz.jiagoushi.top/gtqxobrojn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.guannengcc.top/gtzrzfwszo.html

[S25] C：内存拷贝
来源：http://hz.hammf.cn/gtnqojblmt.html

memcpy(dst, src, n);
来源：http://hz.xziqi.cn/gtfazcnrht.html

[S26] C：内存清零
来源：http://hz.birdmap.top/gtlnflpsho.html


<!-- 参考信息 -->