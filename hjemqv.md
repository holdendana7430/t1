代发 wailian999

[Q63] 开启事务
来源：http://hz.jqgfzy.top/gtdommlisw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cheryme.top/gtfftnbphj.html

[Q64] 提交事务
来源：http://hz.feifeiyinyue.top/gtutnhcudk.html

COMMIT;
来源：http://hz.yj20258888.top/gtrauirlks.html

[Q65] 回滚事务
来源：http://hz.aizwys.cn/gtgxzhbcjv.html

ROLLBACK;
来源：http://hz.jlsjyb.cn/gtnxrfclch.html

[Q66] 行锁查询
来源：http://hz.fengsongda.top/gtgxheqhgz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hnqzz.top/gtmwgtjzfa.html

[Q67] 设置隔离级别
来源：http://hz.shzxlz.cn/gtzwvabkpt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jiagoushi.top/gtpvajjwer.html

[Q68] 保存点
来源：http://hz.guowangkeji.top/gtjynzszmn.html

SAVEPOINT sp1;
来源：http://hz.chenlongwang.top/gtmnrgefae.html

ROLLBACK TO sp1;
来源：http://hz.aizwys.cn/gtfiqpxodg.html

[Q69] 查看执行计划
来源：http://hz.tanke756.top/gtmdodlkjn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.cdnleiting.top/gtjbemsxkm.html

[Q70] 更新统计信息
来源：http://hz.jlsjyb.cn/gtwfghqrlh.html

ANALYZE TABLE users;
来源：http://hz.yvedp.cn/gtqffhvrmy.html

[Q71] 查看建表语句
来源：http://hz.aizwys.cn/gtvnwlawrv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.guowangkeji.top/gtvhhwueoh.html

[Q72] 查看索引
来源：http://hz.meibo888.top/gtsymlezyn.html

SHOW INDEX FROM users;
来源：http://hz.nanxuanxn.top/gtlsqcjcnr.html

[Q73] 查看表状态
来源：http://hz.shuidangran.top/gtjlzyjciy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.xingfuxueyuan.xyz/gtapfbikhj.html

[Q74] 强制使用索引
来源：http://hz.yangfankeji.com/gtvzaqcwda.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.haohaochexian.top/gtkpfjdahc.html

[Q75] 日期格式化
来源：http://hz.ybcxt.top/gtiawklgcr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtkdhlizvg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.wangdashe.top/gtmmgatuaq.html

[Q76] 按天统计
来源：http://hz.redwolf501.top/gttdvywpdt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.chenjidiqi.icu/gtjlicgopy.html

[Q77] 时间加减
来源：http://hz.316326.xyz/gtwjqoqgqc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.quarkkingdee.top/gtpdzdpwig.html

[Q78] 当前时间
来源：http://hz.ehwqpu.com/gtpycdixym.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yanxiufei.cn/gtpeniezow.html

[Q79] 字符串拼接
来源：http://hz.zhixingplan.top/gtlwaouyrg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yuanzhike.top/gtnkqamdqg.html

[Q80] 字符串截取
来源：http://hz.nanxinkj.top/gtbqnuabxq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.fzhhl.top/gtopthiqez.html

[Q81] 字符串替换
来源：http://hz.sweek.top/gtnqhrvbgn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.daria6918.cn/gtqkuedmpl.html

[Q82] 字符长度与字节长度
来源：http://hz.jinqigfzy.top/gteuhhlgpj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtnvyimcgf.html

[Q83] 大小写转换
来源：http://hz.nwbrower.top/gtbrxgojhf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.smart0.xyz/gtfbeduqxm.html

[Q84] 去除首尾空格
来源：http://hz.ivvv.top/gtlxsvmefq.html

SELECT TRIM(name) FROM users;
来源：http://hz.shuidangran.top/gtwxbsazhp.html

[Q85] 数值取整
来源：http://hz.xinyue.icu/gtyhnzvhfn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.haohaochexian.top/gtdyraygrx.html

[Q86] 读取 JSON 字段
来源：http://hz.sweek.top/gtvmwybqwk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jinqigufen.top/gtrepvfigb.html

[Q87] JSON 字段做条件
来源：http://hz.zhoulong.xyz/gtxngdfwfm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.birdmap.top/gtnqwzlzmn.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhoulong.xyz/gtsyhhkpsu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhengqikj.top/gtbnjzgjmv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cqqwz.cn/gtnjqjzkbz.html

[Q89] 判断表是否存在
来源：http://hz.yuanzhike.top/gtqychwxrn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.cdnleiting.top/gtoxjlecfn.html

[Q90] 生成序号列
来源：http://hz.hnqzz.top/gtkifkxizv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.sufxvd.cn/gtlhmxtgfp.html

================================================================================
来源：http://hz.vqdsnc.cn/gtssnkqtag.html

R. Bash 专题
来源：http://hz.ydzc1.top/gtklzvsxmb.html

================================================================================
来源：http://hz.hfpthk.cn/gtekbnivdj.html

[R01] shebang 与严格模式
来源：http://hz.shuidangran.top/gtktpoeloo.html

#!/usr/bin/env bash
来源：http://hz.tanke756.top/gtlkyazjno.html

set -euo pipefail
来源：http://hz.daxiang520.top/gtdbtrdvee.html

[R02] 变量赋值与使用
来源：http://hz.meibo888.top/gtuszxpolg.html

name="Tom"; echo "$name"
来源：http://hz.jinqigufen.top/gtdkvpkddc.html

[R03] 只读变量
来源：http://hz.yj20258.top/gtaxxlnpcp.html

readonly PI=3.14
来源：http://hz.9152youxi.cn/gtvnregttl.html

[R04] 位置参数
来源：http://hz.svipenyu.cn/gtplsnynis.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xziqi.cn/gtliszquqz.html

[R05] 参数默认值
来源：http://hz.zhongyouzk.top/gtslqzmazc.html

name="${1:-default}"
来源：http://hz.ydjk.org.cn/gtoxmjkbxh.html

[R06] 判断命令是否存在
来源：http://hz.zhijiandao.cn/gtmfxpdoqo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.nanxinkj.top/gtyqaoqfen.html

[R07] if 判断文件
来源：http://hz.hnqzz.top/gtqywuubgj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ydzc1.top/gtmkxoyknw.html

[R08] 数值比较
来源：http://hz.pengpengdd.cyou/gtojjboefo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ywan-chungtsiang.top/gthibqaaar.html

[R09] 字符串比较
来源：http://hz.0kj1m.cn/gtxvpemqkr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xinyue.icu/gtkjrbjror.html

[R10] 正则匹配
来源：http://hz.yj20258888.top/gtrzxmrkwk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xylfe.cn/gthbclkfzk.html

[R11] case 多分支
来源：http://hz.zhongyouzk.top/gtljnfznqh.html

case "$1" in
来源：http://hz.hysaishi.cn/gtvbotomqj.html

start) echo "启动" ;;
来源：http://hz.gzhubu.top/gtjqlkhxjo.html

stop)  echo "停止" ;;
来源：http://hz.zhengqikj.top/gtmvpqlupf.html

*)     echo "未知命令" ;;
来源：http://hz.fzhhl.top/gtbgujvioe.html

esac
来源：http://hz.bjfxy.top/gtedejvsqg.html

[R12] for 遍历文件
来源：http://hz.zhoulong.xyz/gtsinuhdfo.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ppjwa.cn/gtlgvzieob.html

[R13] for 计数循环
来源：http://hz.jqgfzy.top/gtkiojmomr.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shzxlz.cn/gtfxkgayed.html

[R14] C 风格 for
来源：http://hz.yanxiufei.cn/gtuycjsqlu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.c1oappe.top/gtsmljpdwl.html

[R15] while 逐行读文件
来源：http://hz.jinqigufen.top/gtnzgtekrr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ydjk.org.cn/gtnkxqgqhy.html

[R16] until 等待条件
来源：http://hz.fzhhl.top/gtmxeyzefr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zdqjudy.top/gtpqonixqx.html

[R17] 数组定义与取值
来源：http://hz.hammf.cn/gtrvdmprbo.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhoulong.xyz/gtevznaizr.html

[R18] 遍历数组
来源：http://hz.iojbl.cn/gtttmokuhz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jlsjyb.cn/gtiyrrhuxy.html

[R19] 数组长度
来源：http://hz.guowangkeji.top/gtvhfpohzc.html

echo "${#arr[@]}"
来源：http://hz.smart0.xyz/gtrzwtsunt.html

[R20] 关联数组（字典）
来源：http://hz.jinqigfzy.top/gtzhdpepbw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.redwolf501.top/gtvgpjxuly.html

[R21] 字符串长度
来源：http://hz.jinyuanbaomall.cn/gtlfbiwrkp.html

echo "${#s}"
来源：http://hz.bjfxy.top/gthhkesuzl.html

[R22] 截取子串
来源：http://hz.daria6918.cn/gttqafjnrr.html

echo "${s:0:5}"
来源：http://hz.jyoumei.cn/gtkvptpnfv.html

[R23] 字符串替换
来源：http://hz.yvedp.cn/gtgqujglup.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.pycfn.com/gtfhvvypfa.html

[R24] 大小写转换
来源：http://hz.bjfxy.top/gtiuiyxyoi.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.fzhhl.top/gtswdumsxu.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhengqikj.top/gtmeakddxf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ivvv.top/gtvdhkcwbi.html

[R26] 命令替换
来源：http://hz.yj202588.top/gtvhyzghoq.html

now=$(date +%F); echo "$now"
来源：http://hz.ydjk.org.cn/gtxsbgyzas.html

[R27] 算术展开
来源：http://hz.ybcxt.top/gtrmjmhwyh.html

echo $((1 + 2 * 3))
来源：http://hz.jianghu66.top/gtrgjpiwul.html

[R28] 浮点运算
来源：http://hz.guannengcc.top/gtzzkvucvt.html

echo "scale=2; 10/3" | bc
来源：http://hz.mhx1999.top/gtqmfzvoxo.html

[R29] 定义函数
来源：http://hz.vqdsnc.cn/gtwwrfahaw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.dianchejie.cn/gtifkdrigg.html

[R30] 函数返回状态码
来源：http://hz.jianghu66.top/gthulhmtkr.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.0kj1m.cn/gthxykcsns.html

[R31] 局部变量
来源：http://hz.c1oappe.top/gtvujtltil.html

f() { local x=1; echo "$x"; }
来源：http://hz.xingfuxueyuan.xyz/gtaojavwxq.html

[R32] 参数个数校验
来源：http://hz.zhengqikj.top/gtppxfsose.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.daria6918.cn/gtiiggzjaq.html

[R33] 捕获错误并提示行号
来源：http://hz.yangfankeji.com/gtfxgvorda.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.sysykeji.top/gtlsvxnusb.html

[R34] 退出时清理
来源：http://hz.haohaochexian.top/gtipkwnuoo.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.havefunace.top/gtlozggmpv.html

[R35] 后台执行并等待
来源：http://hz.dashuyun.cn/gtltfpbqlj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.snrcjt.cn/gtmaqlrrfa.html

[R36] 并发执行多个任务
来源：http://hz.52xcode.cn/gtckemvbzf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhaomingkeji.xyz/gtqaoyshrh.html

[R37] 把输出赋给变量
来源：http://hz.shangyingyoupin.top/gtdofpmact.html

files=$(ls -1)
来源：http://hz.guannengcc.top/gtbnhoqqzv.html

[R38] 管道串联
来源：http://hz.jqgfzy.top/gttfbkguwl.html

cat a.txt | grep -i error | wc -l
来源：http://hz.wangdashe.top/gtgsffdjrn.html

[R39] 重定向标准输出与错误
来源：http://hz.jinqigufen.top/gtysddddwf.html

cmd > out.log 2>&1
来源：http://hz.ivvv.top/gtkvtpydod.html

[R40] 追加写日志
来源：http://hz.tanke756.top/gtasscleoe.html

echo "log" >> out.log
来源：http://hz.zhiwuduotai.top/gtwidqoblj.html

[R41] 丢弃输出
来源：http://hz.zhengqikj.top/gtnesqqalh.html

cmd >/dev/null 2>&1
来源：http://hz.ivvv.top/gtozuhguda.html

[R42] 输入重定向
来源：http://hz.xziqi.cn/gtvitigpuf.html

wc -l < a.txt
来源：http://hz.xuanzx.com/gtivazyrtk.html

[R43] 按名字查找文件
来源：http://hz.jinqigfzy.top/gtpnugqbtc.html

find . -name "*.log" -type f
来源：http://hz.dashuyun.cn/gtbjkvtgor.html

[R44] 按修改时间查找
来源：http://hz.bjfxy.top/gtzpozrqng.html

find . -mtime -7 -type f
来源：http://hz.zhaomingkeji.xyz/gtohvaafff.html

[R45] 批量删除
来源：http://hz.yueranfly.top/gtasgekkpi.html

find . -name "*.tmp" -delete
来源：http://hz.shuidangran.top/gtamfrpkvl.html

[R46] 递归替换文件内容
来源：http://hz.zycfv.cn/gtrrhoktou.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.gogol.net.cn/gtinsexdel.html

[R47] sed 单行替换
来源：http://hz.chenlongwang.top/gtixxqwfhd.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ehwqpu.com/gtguypbjas.html

[R48] awk 取指定列
来源：http://hz.zhiwuduotai.top/gtjosdivhe.html

awk '{print $1, $3}' a.txt
来源：http://hz.yj20258.top/gttapymamo.html

[R49] awk 带条件
来源：http://hz.yueranfly.top/gtaalspmwu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.dianchejie.cn/gtmoocirch.html

[R50] awk 求和
来源：http://hz.xingfuxueyuan.xyz/gtbifjyjwp.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.fzhhl.top/gtkuiwovzt.html

[R51] 排序去重取前几
来源：http://hz.hysaishi.cn/gtapftnzbd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ehwqpu.com/gtagqeciqj.html

[R52] 统计行数
来源：http://hz.nanxinkj.top/gtvqjpdnhc.html

wc -l a.txt
来源：http://hz.jinqigfzy.top/gtlfobuwrj.html

[R53] 查看文件头与实时尾
来源：http://hz.jianghu66.top/gtajarerfe.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shanyushiyangtech.top/gthfewyycb.html

[R54] 比较两个文件
来源：http://hz.hfpthk.cn/gttsbrswdb.html

diff a.txt b.txt
来源：http://hz.meibo888.top/gtxicixkig.html

[R55] 压缩与解压
来源：http://hz.zhoulong.xyz/gtsewbzcyn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yj20258888.top/gtmnukescq.html

[R56] 远程拷贝
来源：http://hz.feifeiyinyue.top/gtjgffndip.html

scp file user@host:/path/
来源：http://hz.mhx1999.top/gtpamqfmgh.html

[R57] 远程执行命令
来源：http://hz.shanyushiyangtech.top/gtjcqypzrw.html

ssh user@host 'uptime'
来源：http://hz.pycfn.com/gtmxeumhoh.html

[R58] 下载文件
来源：http://hz.chenlongwang.top/gtkqcozfey.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinqigfzy.top/gtvzokxtry.html

[R59] 发 POST JSON
来源：http://hz.smart0.xyz/gtypunabhx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xuetiantiany.cn/gtexoxifxj.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhoulong.xyz/gtdzbjzhrq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xylfe.cn/gtyldcxztl.html

[R61] 磁盘占用
来源：http://hz.iojbl.cn/gtlgjhrnyt.html

df -h;  du -sh *
来源：http://hz.daxiang520.top/gttmrdperw.html

[R62] 找最占空间的文件
来源：http://hz.zycfv.cn/gtpsvkslyz.html

du -ah . | sort -rh | head -10
来源：http://hz.ivvv.top/gtvnhfngfu.html

[R63] 内存与进程
来源：http://hz.ydzc1.top/gtsfnktygj.html

free -h;  ps aux | grep nginx
来源：http://hz.wangshuangyany.cn/gtctaxakvi.html

[R64] 结束进程
来源：http://hz.ydjk.org.cn/gtpolxqhbc.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sxryk.cn/gttxiypitz.html

[R65] 查看端口占用
来源：http://hz.jinghuilouyu.cn/gtvyoqldtk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.aizwys.cn/gtyxqksjyr.html

[R66] 定时任务
来源：http://hz.redwolf501.top/gtmhvrolgk.html

crontab -e;  crontab -l
来源：http://hz.tianlin.xyz/gtvdbkonqh.html

[R67] 生成随机十六进制串
来源：http://hz.smart0.xyz/gtrlrgdrkq.html

openssl rand -hex 16
来源：http://hz.zdqjudy.top/gtbgaftkbb.html

[R68] 计算文件校验值
来源：http://hz.sweek.top/gttmhjnirz.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhijiandao.cn/gtjnnonfwe.html

[R69] 生成随机密码
来源：http://hz.iojbl.cn/gtjnrnxudj.html

head -c 16 /dev/urandom | base64
来源：http://hz.hongshengwenyu.top/gtkpsylvml.html

[R70] 时间戳与互转
来源：http://hz.shanyushiyangtech.top/gtrtzkjkmv.html

date +%s;  date -d @1700000000
来源：http://hz.gogol.net.cn/gtaclscdhq.html

[R71] 日期格式化
来源：http://hz.daria6918.cn/gtvudfaaem.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.0kj1m.cn/gtfaaerkkd.html

[R72] 等待端口就绪
来源：http://hz.jqgfzy.top/gtmhwjrsjo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yonumen.top/gtvkkpzytc.html

[R73] 分割大日志
来源：http://hz.shanyushiyangkeji.top/gtlmmahbkc.html

split -l 1000 big.log part_
来源：http://hz.snrcjt.cn/gtpsztxwzz.html

[R74] 批量重命名
来源：http://hz.daxiang520.top/gtwnvzyvdv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jqgufenzy.top/gtvwazycuo.html

[R75] 导出环境变量
来源：http://hz.9152youxi.cn/gtilagqmbu.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.wangshuangyany.cn/gthlkwnbbx.html

[R76] 使用临时文件
来源：http://hz.nanxinkj.top/gtuluabdee.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinghuilouyu.cn/gtqjqecyue.html

[R77] 读取用户输入
来源：http://hz.dashuyun.cn/gtowicdxbl.html

read -rp "请输入: " ans
来源：http://hz.guannengcc.top/gtvxricfdw.html

[R78] 交互式菜单
来源：http://hz.cqqwz.cn/gtcnmvpgbn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xingfuxueyuan.xyz/gtlfzaokgk.html

[R79] 解析命令行选项
来源：http://hz.sufxvd.cn/gtkstlijwa.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.guannengcc.top/gtchenlvad.html

[R80] 查看脚本执行耗时
来源：http://hz.sufxvd.cn/gtreelvuou.html

time ./run.sh
来源：http://hz.jinghuilouyu.cn/gtdpslwzcs.html

================================================================================
来源：http://hz.yangfankeji.com/gtdjlfuciy.html

S. C / C++ 专题
来源：http://hz.zhiwuduotai.top/gtmusdnvap.html

================================================================================
来源：http://hz.birdmap.top/gtuqkbdgng.html

[S01] C：Hello World
来源：http://hz.jqgufenzy.top/gtnuffrsto.html

#include <stdio.h>
来源：http://hz.fengsongda.top/gtmkrcmyaf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yangfankeji.com/gtjtnlaoot.html

[S02] C：变量与格式化输出
来源：http://hz.jlsjyb.cn/gtkaingvlc.html

int a = 10; printf("%d\n", a);
来源：http://hz.shangyingyoupin.top/gtkzmieleo.html

[S03] C：读入整数
来源：http://hz.ehwqpu.com/gtiyqdwtar.html

int x; scanf("%d", &x);
来源：http://hz.sufxvd.cn/gtveneuhob.html

[S04] C：字符串复制
来源：http://hz.birdmap.top/gtvnwprnfd.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinyuanbaomall.cn/gtcyuekjxv.html

[S05] C：字符串长度
来源：http://hz.dianchejie.cn/gtmlkxqgly.html

strlen(s)
来源：http://hz.shanyushiyangkeji.top/gtmjvpugfl.html

[S06] C：字符串比较
来源：http://hz.pengpengdd.cyou/gtmxcubgcs.html

strcmp(a, b) == 0
来源：http://hz.gzhubu.top/gtelohisva.html

[S07] C：数组遍历求和
来源：http://hz.guannengcc.top/gtiripezar.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.aizwys.cn/gttccwhlhy.html

[S08] C：动态内存分配与释放
来源：http://hz.nanxinkj.top/gtjbtrgmqh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.daxiang520.top/gtvistnukx.html

[S09] C：结构体定义与初始化
来源：http://hz.jqgufenzy.top/gtbuvzvepy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cdnleiting.top/gtswwsraef.html

[S10] C：指针与解引用
来源：http://hz.jiagoushi.top/gtljfhnucw.html

int *p = &a;  *p = 5;
来源：http://hz.shanyushiyangtech.top/gtduquzeob.html

[S11] C：逐行读文件
来源：http://hz.bjfxy.top/gtsrjlarcz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shangyingyoupin.top/gtiypkrikc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.iojbl.cn/gtfytlwxga.html

fclose(f);
来源：http://hz.0kj1m.cn/gtpypttldd.html

[S12] C：写文件
来源：http://hz.hysaishi.cn/gtuprilqjk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.kuanghao11.cn/gtzlavahqz.html

[S13] C：宏定义
来源：http://hz.shzxlz.cn/gtdewawpbe.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.svipenyu.cn/gtipvbwlte.html

[S14] C：枚举
来源：http://hz.xingfuxueyuan.xyz/gtkzxkmgof.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.dianchejie.cn/gtdcrjldao.html

[S15] C：类型转换
来源：http://hz.dashuyun.cn/gtvyplndij.html

(double) a / b
来源：http://hz.fengsongda.top/gtyhntqwij.html

[S16] C：位操作置位
来源：http://hz.gogol.net.cn/gtxduxtmhl.html

x |= (1 << 3);
来源：http://hz.xuetiantiany.cn/gtcvrdpgat.html

[S17] C：安全拼接字符串
来源：http://hz.ppjwa.cn/gtfoeyymzj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinghuilouyu.cn/gtvyoepfdd.html

[S18] C：命令行参数
来源：http://hz.guowangkeji.top/gtoadyimxc.html

int main(int argc, char **argv)
来源：http://hz.ywan-chungtsiang.top/gtmkyinjsu.html

[S19] C：快速排序
来源：http://hz.havefunace.top/gtjriwcmsl.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.tianlin.xyz/gtwionlaom.html

[S20] C：二分查找
来源：http://hz.pengpengdd.cyou/gtijcvhfev.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ivvv.top/gtjwsrrnfn.html

[S21] C：字符类别判断
来源：http://hz.shanyushiyangtech.top/gtequextom.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.meibo888.top/gtyjzkqaqz.html

[S22] C：字符串转数字
来源：http://hz.zdqjudy.top/gtwxyiylbv.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ybcxt.top/gtmooyhnnx.html

[S23] C：随机数
来源：http://hz.daria6918.cn/gtvteaceol.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.havefunace.top/gtgswlzber.html

[S24] C：获取本地时间
来源：http://hz.yanxiufei.cn/gtgoyxxdqe.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.sxryk.cn/gtrxnvywwu.html

[S25] C：内存拷贝
来源：http://hz.xinyue.icu/gtrasrszru.html

memcpy(dst, src, n);
来源：http://hz.0kj1m.cn/gtbbmwbvlx.html

[S26] C：内存清零
来源：http://hz.ydzc1.top/gtmjdgonbn.html

memset(a, 0, sizeof a);
来源：http://hz.chenzaomai.com/gtrthjikgq.html

[S27] C：定义常量
来源：http://hz.wangdashe.top/gtgvdpzkhb.html

const double PI = 3.14159;
来源：http://hz.yj20258.top/gtbfsqlotj.html

[S28] C：静态变量
来源：http://hz.cqqwz.cn/gtbkblmynz.html

static int counter = 0;
来源：http://hz.yj20258888.top/gtrjmcrhva.html

[S29] C：变参函数
来源：http://hz.jyoumei.cn/gteijplidr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xziqi.cn/gtmzigrhrz.html

[S30] C：头文件保护
来源：http://hz.ivvv.top/gtlhojhoiw.html

#ifndef X_H
来源：http://hz.zdqjudy.top/gtaqdzdvpu.html

#define X_H
来源：http://hz.nanxinkj.top/gtzjfihies.html

#endif
来源：http://hz.meibo888.top/gtzvxzyhtm.html

[S31] C++：Hello World
来源：http://hz.guannengcc.top/gtbzxrvsmd.html

#include <iostream>
来源：http://hz.wangdashe.top/gtraakskgt.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.chenjidiqi.icu/gtgycmavxf.html

[S32] C++：字符串
来源：http://hz.9152youxi.cn/gtdubzmeml.html

std::string s = "hi";  s += "!";
来源：http://hz.shanyushiyangtech.top/gtdrvvafua.html


<!-- 参考信息 -->