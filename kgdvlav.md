代发 wailian999

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gxcwxckao.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/ggumsybaq.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/godgtlgwu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gfgftjuio.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gjkdwjfte.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/ggllwpusc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gccgwqmwy.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/ggwuiuwrt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gsdqdfzhr.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/ghruxnokm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gueixmgtj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggllwqhpu.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gwyqrowqp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gziriolun.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/ggcbqvlwo.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gjkbeylhy.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/glwzrkipx.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gjzuznbcx.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gtrbtzigs.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gkzveiuac.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gnkiyxwal.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gpfgvmpss.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/giwzzdabx.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/ggdhvgzft.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gmydggqkt.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gtekqudhq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gcpevwyiw.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gfodtwzcp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/graesgagt.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gclpuezjv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gwqwgluie.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gzaetugtu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gqekkdcxw.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/geeikzxlw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gzlimuals.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gvavprqch.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gompeufwm.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/grzctofca.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gocaalmgk.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gifofzedm.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/ggziduvbf.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gkuiwukcf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gbhuvawhr.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/giczwrphj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gpuscujjp.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gixsszcii.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gqoqphsfr.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gcurmkbad.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/grrdhreuf.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/goegedztj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gasnacbir.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gawrvlgie.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gyuqmfgze.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gigqgatfe.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/grmbamuql.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gutqskrpz.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gkajvafmr.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gpeaslcca.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/gloxtnptx.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gdzqjeeax.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gdjytimbr.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/ggbvckfry.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gycgxrzdl.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gukckkglz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gpuczxuib.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/geklocmsl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gazpxsvut.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gfmhhnsnr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gdclpgvvb.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gxswntzrz.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/giklrvbok.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gysfdacbt.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gexaxscaz.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gjkvgczjo.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gfftfpfdi.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gxolrfmma.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gwkabmhma.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gggdonhap.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gwchruhwe.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gvpcdldtb.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gzhlghxgb.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/ghwquzugo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gyeapxhqh.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/ggsvgnqmv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/ghagaqzga.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/geebfzgyf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gsoaxzcyz.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/goadtrlge.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gtfpkdgqx.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gyotjioej.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/ghtfdjicf.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gwmbeoxkj.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/giuswdlhy.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gaeotgnzl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gdudcerug.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/grdxgnhng.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gxqzenqms.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gvfekoqaj.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/ggsyyfbeo.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/gdfstvkcw.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gexgbxlvm.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/geepcpevp.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gyetvlcny.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gyawvrary.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gmwbuoacf.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/grashdrjd.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gyfetqrlf.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gfkeugkuz.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/giqacyuhf.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gvawtyndv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gpzxzxmkb.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/ggefyqvzh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gptciqjqb.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gweejasfo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gntdbtkzw.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gvqhhbbyx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/glsunrbrh.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gwqomhqni.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gudsayeit.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gwjtbemaj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gvjrmnodz.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gtqhftyru.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gnpjfggpj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gpshufxrm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/giafgewvh.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/ghiqvwvxr.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gkclrkbkw.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gpaylzahp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gqcriqefc.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gzjobzsfg.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/guqifpski.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/garacftfw.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gxqdvqpdd.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gcbfgncsf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gqgxqfutc.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gtzhlagks.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gfqaekwkv.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gbrfaxkui.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gzjgwqcxh.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gkthkgpdh.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gyjhxuvdp.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gksqzlxnf.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gzqzjyoju.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gvrkbfyrn.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/glmgmzrra.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gboidtxbr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gaouxnhtw.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/grjlymyrb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/grdrcpiod.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/gmteafdpt.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gbyiemiwj.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gacnzoekm.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gzltrcgjs.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gytyblwis.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/giahfnnrp.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gzohihtog.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gzvzqbzvp.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gznfaubci.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gqdbdqmuv.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gzdniwknk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gmkxylewt.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/goaalvjfz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gawqdhpzr.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gxhnlabjf.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/goqmhhstf.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gqvcjaxew.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gouwquetr.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/grxalkxgp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gfcsfeuur.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gvzgnvmcu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/goyqxupri.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/ghhsxmltc.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gpqaiczvt.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gfhyrzpkm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/ghtnxtvih.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gptamjmvy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gkaxottwc.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gnzgokoya.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gcqcdxzou.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gckmvslxx.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/glpdoahga.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbxgjieae.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gkgythmat.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/goxeelzru.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gxphqjfgc.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gwylawbzc.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gfgudzsuv.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gbuffcmjz.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gtrefxmek.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gjaepnqcy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gpdebxixn.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gdscxgbqf.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gcukwhjqr.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gjvpororu.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gavwkbqsd.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gathewckt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/ggpvxllae.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gtwxmdnmc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gmgyfurxa.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gyquuhtth.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gwhhfvcbc.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gkjfxdysu.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gejicugkr.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gwgcldqhu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gbdqwjprh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/ghxolufzb.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/grzaztfth.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/grupvvlyb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gppidanaq.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/ggsplmtav.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gfnifttqc.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gubmqfjet.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gprleolyl.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gksiquwia.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gvburxmlr.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/ghgwquplz.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gslapqled.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gamtkkxrx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/grdciugax.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gkaanvnvh.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/ghbqabruy.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/giiyzckbb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gviycgqed.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gercnbmkk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gfxqbzvrl.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/guknbjvym.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gqrwcfbue.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/girhtemoi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gdedecdwi.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gkgerfjwk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gkhatgcuq.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gedrvrakw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gwdqnfzgn.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gxdsqaknw.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gqvkgrcpc.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gcgfqbofh.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gfpjoliik.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gkbueyqtm.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/guehdjpas.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gngyzwclw.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/grsnddqbx.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/goqattekn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gixcdxwkn.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/ghieciibn.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gjqllrvjm.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gkawzpokj.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gsbdffngu.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/giosmjwvt.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gkwswgqva.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gfnsfwesh.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gfwiybsia.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gcixeihhw.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gzoxgoops.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/ghetzjxbh.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gnozhsyba.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gnymxwnzc.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gmgawnqzu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gkydgnjfn.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/ggkxxeaje.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/ghimlmbos.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/goagbaehh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gvsvgwlbs.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gwytwmowk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gdwgedylr.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gnolezpyf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gnsgtdixe.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gcqgjojym.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gulfuomjh.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gjezunchd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gsxmdhsum.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gttrfgyds.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gzowakicy.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gdlocyrci.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gtbeunujl.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gqrekixgp.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gekrwxrih.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gmlhagqzx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gdsztzsfb.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gqlnsbftc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gtkeykugr.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gpfgqgffp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gqwmawahz.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/grqkcfbrz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gnhnehwld.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gvhvifphs.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/ggindhvmw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gzjsucxli.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/ghteohjka.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gxwjexpxb.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/glifcfptd.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gdezccvou.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gekhwusuz.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gewwrjwsd.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gegwpsiot.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gtvpbgjxp.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/ghtukcihr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gphfgodbg.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gfebhoeok.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gdgdufrve.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gpvflnoov.sHtML


<!-- 参考信息 -->